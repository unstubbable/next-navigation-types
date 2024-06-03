Reproducing a compiler issue with `next/navigation-types/compat/navigation`

## Install

`pnpm i`

## Build & Compile

`pnpm build`

Result:

```
  ▲ Next.js 15.0.0-canary.7

   Creating an optimized production build ...
 ✓ Compiled successfully
   Linting and checking validity of types  .Failed to compile.

./node_modules/.pnpm/next@15.0.0-canary.7_react-dom@19.0.0-rc-f994737d14-20240522_react@19.0.0-rc-f994737d14-20240522/node_modules/next/navigation-types/compat/navigation.d.ts:11:19
Type error: Overload signatures must all be exported or non-exported.

   9 |    * ready.
  10 |    */
> 11 |   export function useSearchParams(): ReadonlyURLSearchParams | null
     |                   ^
  12 |
  13 |   /**
  14 |    * Get the current pathname. For example, if the URL is
 ELIFECYCLE  Command failed with exit code 1.
```
