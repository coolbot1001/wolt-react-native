# expo react-native wolt

```bash
npx create-expo-app@latest wolt
```

## codebase

https://github.com/Galaxies-dev/wolt-react-native

## install base

```bash
# font
# https://github.com/expo/google-fonts
# https://fonts.google.com/?query=nunito
npx expo install @expo-google-fonts/nunito expo-font

# https://docs.expo.dev/versions/latest/sdk/haptics/
# 一个库，提供访问系统振动效果的 Android 库、iOS 上的触觉引擎以及网页上的 Web Vibration API。
npx expo install expo-haptics

# https://docs.expo.dev/versions/latest/sdk/ui/
# 目前最新版本是 ~0.2.0-beta.9
npx expo install @expo/ui@~0.2.0-beta.7

# 数据管理
npx expo install zustand
npx expo install react-native-mmkv react-native-nitro-modules

# 数据请求
npx expo install @tanstack/react-query

```

## 初始化基础数据

### assets

- images 提供logo，模拟数据的图片等

### data

categories.ts：美食分类，主要用于筛选和展示。
restaurants.ts：所有餐馆的详细信息。
restaurant_menu.ts：某个餐馆的菜单明细，通常以餐馆名称或 id 命名变量。
restaurant_markers.ts：餐厅的坐标位置，用于地图展示。

### service

没有使用到后端，模拟获取数据

### hooks

页面获取数据的钩子函数

### constants

- theme.ts 用于设置主题

### 预构建

```bash
npx expo prebuild --platform ios
npx expo run:ios

npx expo prebuild --platform android
```

### coderabbit

[docs](https://docs.coderabbit.ai/guides/commands#manually-request-code-reviews)

如果没有在 pr 的时候进行检查，可以在pr里添加这个注释`@coderabbitai full review`
