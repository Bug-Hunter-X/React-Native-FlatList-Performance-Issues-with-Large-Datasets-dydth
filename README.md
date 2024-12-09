# React Native FlatList Performance Optimization

This repository demonstrates a common performance issue with React Native's FlatList component when rendering a large number of items and provides a solution for improved performance.

## Problem

Rendering a large dataset in a FlatList can lead to poor performance, causing slow rendering, unresponsiveness, and potential crashes.

## Solution

The solution involves several techniques to optimize rendering:

1. **Item Optimization:** Simplify the rendering of each list item to reduce computational overhead.  Avoid unnecessary calculations and rendering within each item.
2. **Window Size Optimization:** Adjust the `windowSize` prop to control how many items are rendered at once. A smaller window size reduces initial render time but might impact smooth scrolling.
3. **Virtualization:** FlatList already handles virtualization, but ensure your data structure and rendering are optimized to fully leverage this functionality. Avoid over-rendering of off-screen items.

## How to Run

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `react-native run-android` or `react-native run-ios` to run the app on your device or simulator.