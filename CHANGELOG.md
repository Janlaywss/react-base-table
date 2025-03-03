# CHANGELOG

## NEXT VERSION

## v1.13.0 (2021-10-24)

- fix: change propTypes for `BaseTable.components`
- feat: add support for React 17

## v1.12.0 (2020-10-11)

- feat: add the ability to pass function in `estimatedRowHeight` to determine the initial height of rows

## v1.11.3 (2020-08-24)

- fix: remove propTypes for Column.key

## v1.11.2 (2020-08-18)

- fix: add missing types for propTypes of `BaseTable`

## v1.11.1 (2020-08-17)

- fix: add types folder into packages
- chore: mark `Column.key` as required

## v1.11.0 (2020-08-17)

- feat: add `ignoreFunctionInColumnCompare` to solve closure problem in renderers
- chore: skip unnecessary cloneElement in `renderElement`
- feat: add type declarations

## v1.10.9 (2020-08-13)

- fix: input loses focus on unmount

## v1.10.8 (2020-08-11)

- fix: scroll position would be reset to top if column becomes frozen

## v1.10.7 (2020-07-28)

- fix: `getTotalRowsHeight` could be different before/after render in dynamic mode on initial render

## v1.10.6 (2020-07-25)

- fix: `getTotalRowsHeight` could be different before/after render in dynamic mode

## v1.10.5 (2020-07-10)

- chore: do not clear row height cache automatically

## v1.10.4 (2020-07-02)

- fix: flicker on expanding in dynamic mode

## v1.10.3 (2020-06-30)

- fix: horizontal scrollbar in flex mode with dynamic row height
- chore: tweak row height measurement

## v1.10.2 (2020-06-26)

- fix: regression of expansion with frozen columns
- fix: dynamic rowHeight is not updated when `data` or `columns` changed

## v1.10.1 (2020-06-24)

- fix: dynamic rowHeight is not calculated correctly with frozen columns
- fix: dynamic rowHeight is not updated when resizing column

## v1.10.0 (2020-06-22)

- feat: add `estimatedRowHeight` to support dynamic row height

## v1.9.4 (2020-06-22)

- chore: loosen prop type check for `data`

## v1.9.3 (2020-05-26)

- fix: wrong description for Column props

## v1.9.2 (2020-04-22)

- fix: frozen data not shown with empty data

## v1.9.1 (2019-10-17)

- reverted #80, now custom renderer doesn't support top level hooks, see #109

## v1.9.0 (2019-09-24)

- feat: add `onColumnResizeEnd` prop to `BaseTable`

## v1.8.1 (2019-09-23)

- fix: `unflatten` should not override the existing children

## v1.8.0 (2019-08-30)

- feat: remove deprecated lifecycles for concurrent mode ready

## v1.7.3 (2019-08-27)

- fix: fix possible memory leak in `ColumnResizer`
- fix: bring back column resize on touch events support

## v1.7.2 (2019-08-26)

- ~~fix: custom renderers should support function component with hooks~~

## v1.7.1 (2019-08-22)

- fix: `scrollToRow` doesn't work regression introduced in #73

## v1.7.0 (2019-08-06)

- chore: remove the use of `Object.values`
- feat: add `getColumnManager` and `getDOMNode` methods

## v1.6.5 (2019-07-11)

- fix: style value `unset` is not supported on IE

## v1.6.4 (2019-07-09)

- fix: content been selected when dragging on IE/FF (regression from #56)

## v1.6.3 (2019-07-09)

- fix: `minWidth` is passed to dom node in `ColumnResizer` in #56

## v1.6.2 (2019-07-07)

- fix: `getValue` returns the object itself if the path is not valid string

## v1.6.1 (2019-07-06)

- feat: support infinite loading with `maxHeight`
- chore: remove unused `$table-border-radius` variable
- feat: add `sortState` to support multi sort

## v1.5.0 (2019-07-06)

- refactor: remove dependent on `react-draggable`
- fix: undefined parentId should be considered as root item
- fix: `flattenOnKeys` not works with immutable data (regression from #23)

## v1.4.0 (2019-07-01)

- refactor: remove dependent on `lodash`, and export `getValue`
- build: use `@babel/plugin-transform-runtime` to reduce bundle size

## v1.3.3 (2019-06-27)

- fix: use `PropTypes.elementType` for `tagName`'s type

## v1.3.2 (2019-06-14)

- fix: resizing line rendered incorrectly when resizing the right frozen column

## v1.3.1 (2019-06-06)

- chore: upgrade `react-window` to silence the deprecation

## v1.3.0 (2019-05-10)

- feat: allow `rowKey` to be `number`
- feat: add `getScrollbarSize` to `BaseTable` to custom scrollbar size measurement

## v1.2.2 (2019-05-03)

- perf: optimize `unflatten` and `flattenOnKeys` to not use recursion

## v1.2.1 (2019-05-01)

- fix: scrollbar size don't updated in SSR

## v1.2.0 (2019-04-29)

- chore: more accurate `onScrollbarPresenceChange`
- feat: replace `react-virtualized` with `react-window`
- feat: add scroll direction to `onScroll`
- feat: add `align` to `scrollToRow`

## v1.1.1 (2019-04-27)

- fix: `flattenOnKeys` memoize is opt out because `this._depthMap` changes everytime
- fix: hover state is out of sync in frozen rows, regression introduced in #9

## v1.1.0 (2019-04-26)

- chore: stop using `Grid` for table's header
- chore: add `role` to table's elements
- chore: stop using `forceUpdate` to update the table
- fix: table's header is re-rendered unnecessarily on row hovered

## v1.0.2 (2019-04-03)

- fix: `onScroll` is called redundantly if there are frozen columns

## v1.0.1 (2019-03-28)

- fix: header row's height doesn't update on `headerHeight` change

## v1.0.0 (2019-03-26)

Initial public release
