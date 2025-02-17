# React Native FlatList: Duplicate Keys in keyExtractor

This repository demonstrates a common error in React Native's `FlatList` component: using duplicate keys in the `keyExtractor` function.  Duplicate keys lead to unpredictable behavior and crashes.  The solution focuses on ensuring unique keys for each item.

## Bug Description
The `FlatList` component requires unique keys for efficient rendering and data management.  If the `keyExtractor` function returns the same key for different items, it will cause inconsistencies, unexpected rendering, and even app crashes.

## Solution
The solution involves carefully crafting a `keyExtractor` function that generates unique keys based on data properties or a unique identifier.