### Error in Next js App ROuter

### used tech

- Nextjs app router
- Ant design
- Redux
- axios for RTK query

# My Error is in console >>>

```js
Warning: Extra attributes from the server: data-new-gr-c-s-check-loaded,data-gr-ext-installed
    at body
    at html
    at StyleProvider (webpack-internal:///(app-pages-browser)/./node_modules/@ant-design/cssinjs/es/StyleContext.js:69:24)
    at StyledComponentsRegistry (webpack-internal:///(app-pages-browser)/./src/lib/AntdRegistry.tsx:14:11)
    at Provider (webpack-internal:///(app-pages-browser)/./node_modules/react-redux/es/components/Provider.js:13:3)
    at Providers (webpack-internal:///(app-pages-browser)/./src/lib/Providers.tsx:15:11)
    at RedirectErrorBoundary (webpack-internal:///(app-pages-browser)/./node_modules/next/dist/client/components/redirect-boundary.js:72:9)
    at RedirectBoundary (webpack-internal:///(app-pages-browser)/./node_modules/next/dist/client/components/redirect-boundary.js:80:11)
    at NotFoundErrorBoundary (webpack-internal:///(app-pages-browser)/./node_modules/next/dist/client/components/not-found-boundary.js:54:9)
    at NotFoundBoundary (webpack-internal:///(app-pages-browser)/./node_modules/next/dist/client/components/not-found-boundary.js:62:11)
    at DevRootNotFoundBoundary (webpack-internal:///(app-pages-browser)/./node_modules/next/dist/client/components/dev-root-not-found-boundary.js:32:11)
    at ReactDevOverlay (webpack-internal:///(app-pages-browser)/./node_modules/next/dist/client/components/react-dev-overlay/internal/ReactDevOverlay.js:66:9)
    at HotReload (webpack-internal:///(app-pages-browser)/./node_modules/next/dist/client/components/react-dev-overlay/hot-reloader-client.js:287:11)
    at Router (webpack-internal:///(app-pages-browser)/./node_modules/next/dist/client/components/app-router.js:157:11)
    at ErrorBoundaryHandler (webpack-internal:///(app-pages-browser)/./node_modules/next/dist/client/components/error-boundary.js:82:9)
    at ErrorBoundary (webpack-internal:///(app-pages-browser)/./node_modules/next/dist/client/components/error-boundary.js:110:11)
    at AppRouter (webpack-internal:///(app-pages-browser)/./node_modules/next/dist/client/components/app-router.js:440:13)
    at ServerRoot (webpack-internal:///(app-pages-browser)/./node_modules/next/dist/client/app-index.js:123:11)
    at RSCComponent
    at Root (webpack-internal:///(app-pages-browser)/./node_modules/next/dist/client/app-index.js:139:11)

```

### solve of the Error use suppressHydrationWarning={true} in body or <html> ::::

```tsx
<html lang="en">
  <body className={inter.className} suppressHydrationWarning={true}>
    {children}
  </body>
</html>
```

### project url 

https://github.com/sarwar-asik/um-frontend
