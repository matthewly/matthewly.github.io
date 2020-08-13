---
layout: post
title: Containers vs Presentational Components in React
---

Containers
- High level components that should be connected to Redux store.
- Provides the data and behavior to presentational or other container components.
- Usually stateful

Presentational Component
- These components receive data and callbacks via props.
- Gets data from Redux store as second hand
- Mostly concerned with visuals rather than connecting data