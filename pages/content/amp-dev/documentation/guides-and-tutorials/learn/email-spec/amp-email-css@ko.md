---
'$title': 이메일용 AMP 지원 CSS
$order: 5
formats:
  - email
teaser:
  text: 이 문서는 현재 AMP 이메일에서 지원되는 CSS 기능을 간략하게 설명합니다.
toc: 'true'
---

<!--
This file is imported from https://github.com/ampproject/amphtml/blob/main/spec/email/amp-email-css.md.
Please do not change this file.
If you have found a bug or an issue please
have a look and request a pull request there.
-->

<!---
Copyright 2018 The AMP HTML Authors. All Rights Reserved.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

      http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS-IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
-->

이 문서는 현재 AMP 이메일에서 지원되는 CSS 기능을 간략하게 설명합니다.

## CSS 적용 <a name="applying-css"></a>

### 내부 스타일시트 <a name="internal-stylesheet"></a>

내부 스타일시트를 사용할 경우 이메일의 `<head>` 태그에 포함된 단일한 `<style amp-custom>` 태그 내부에 CSS가 지정됩니다.

### 인라인 스타일 <a name="inline-styles"></a>

내부 스타일시트에 추가로 [`style` 속성](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes#attr-style)을 사용하여 모든 요소에 인라인 스타일을 지정할 수 있습니다.

### 외부 스타일시트 <a name="external-stylesheet"></a>

이메일용 AMP에서 외부 스타일시트는 지원되지 **않습니다**.

이메일 어디에도 `<link rel="stylesheet" href="...">`는 허용되지 않습니다.

## 지원되는 CSS 선택자 <a name="supported-css-selectors"></a>

### 단순 선택자 <a name="simple-selectors"></a>

- [유형 선택자](https://developer.mozilla.org/en-US/docs/Web/CSS/Type_selectors) `elementname`
- [클래스 선택자](https://developer.mozilla.org/en-US/docs/Web/CSS/Class_selectors) `.classname`
- [ID 선택자](https://developer.mozilla.org/en-US/docs/Web/CSS/ID_selectors) `#idname`
- [전체 선택자](https://developer.mozilla.org/en-US/docs/Web/CSS/Universal_selectors) `*`
- [속성 선택자](https://developer.mozilla.org/en-US/docs/Web/CSS/Attribute_selectors) `[attr=value]`

### 결합자 <a name="combinators"></a>

- [인접 형제 결합자 ](https://developer.mozilla.org/en-US/docs/Web/CSS/Adjacent_sibling_combinator) `A + B`
- [일반 형제 결합자 ](https://developer.mozilla.org/en-US/docs/Web/CSS/General_sibling_combinator) `A ~ B`
- [자식 결합자](https://developer.mozilla.org/en-US/docs/Web/CSS/Child_combinator) `A > B`
- [자손 결합자](https://developer.mozilla.org/en-US/docs/Web/CSS/Descendant_combinator) `A B`

### 의사 클래스 <a name="pseudo-classes"></a>

- [`:active`](https://developer.mozilla.org/en-US/docs/Web/CSS/:active)
- [`:checked`](https://developer.mozilla.org/en-US/docs/Web/CSS/:checked)
- [`:default`](https://developer.mozilla.org/en-US/docs/Web/CSS/:default)
- [`:disabled`](https://developer.mozilla.org/en-US/docs/Web/CSS/:disabled)
- [`:empty`](https://developer.mozilla.org/en-US/docs/Web/CSS/:empty)
- [`:enabled`](https://developer.mozilla.org/en-US/docs/Web/CSS/:enabled)
- [`:first-child`](https://developer.mozilla.org/en-US/docs/Web/CSS/:first-child)
- [`:first-of-type`](https://developer.mozilla.org/en-US/docs/Web/CSS/:first-of-type)
- [`:focus`](https://developer.mozilla.org/en-US/docs/Web/CSS/:focus)
- [`:focus-within`](https://developer.mozilla.org/en-US/docs/Web/CSS/:focus-within)
- [`:hover`](https://developer.mozilla.org/en-US/docs/Web/CSS/:hover)
- [`:in-range`](https://developer.mozilla.org/en-US/docs/Web/CSS/:in-range)
- [`:indeterminate`](https://developer.mozilla.org/en-US/docs/Web/CSS/:indeterminate)
- [`:invalid`](https://developer.mozilla.org/en-US/docs/Web/CSS/:invalid)
- [`:last-child`](https://developer.mozilla.org/en-US/docs/Web/CSS/:last-child)
- [`:last-of-type`](https://developer.mozilla.org/en-US/docs/Web/CSS/:last-of-type)
- [`:last-of-type`](https://developer.mozilla.org/en-US/docs/Web/CSS/:last-of-type)
- [`:not`](https://developer.mozilla.org/en-US/docs/Web/CSS/:not)
- [`:nth-child`](https://developer.mozilla.org/en-US/docs/Web/CSS/:nth-child)
- [`:nth-last-child`](https://developer.mozilla.org/en-US/docs/Web/CSS/:nth-last-child)
- [`:nth-last-of-type`](https://developer.mozilla.org/en-US/docs/Web/CSS/:nth-last-of-type)
- [`:nth-of-type`](https://developer.mozilla.org/en-US/docs/Web/CSS/:nth-of-type)
- [`:only-child`](https://developer.mozilla.org/en-US/docs/Web/CSS/:only-child)
- [`:only-of-type`](https://developer.mozilla.org/en-US/docs/Web/CSS/:only-of-type)
- [`:optional`](https://developer.mozilla.org/en-US/docs/Web/CSS/:optional)
- [`:out-of-range`](https://developer.mozilla.org/en-US/docs/Web/CSS/:out-of-range)
- [`:read-only`](https://developer.mozilla.org/en-US/docs/Web/CSS/:read-only)
- [`:read-write`](https://developer.mozilla.org/en-US/docs/Web/CSS/:read-write)
- [`:required`](https://developer.mozilla.org/en-US/docs/Web/CSS/:required)
- [`:valid`](https://developer.mozilla.org/en-US/docs/Web/CSS/:valid)

## 지원되는 CSS 속성 <a name="supported-css-properties"></a>

- [`-moz-appearance`](https://developer.mozilla.org/en-US/docs/Web/CSS/appearance)
- [`-webkit-appearance`](https://developer.mozilla.org/en-US/docs/Web/CSS/appearance)
- [`-webkit-tap-highlight-color`](https://developer.mozilla.org/en-US/docs/Web/CSS/-webkit-tap-highlight-color)
- [`align-content`](https://developer.mozilla.org/en-US/docs/Web/CSS/align-content)
- [`align-items`](https://developer.mozilla.org/en-US/docs/Web/CSS/align-items)
- [`align-self`](https://developer.mozilla.org/en-US/docs/Web/CSS/align-self)
- [`appearance`](https://developer.mozilla.org/en-US/docs/Web/CSS/appearance)
- [`azimuth`](https://developer.mozilla.org/en-US/docs/Web/CSS/azimuth)
- [`background`](https://developer.mozilla.org/en-US/docs/Web/CSS/background)
- [`background-attachment`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-attachment)
- [`background-blend-mode`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-blend-mode)
- [`background-clip`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-clip)
- [`background-color`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-color)
- [`background-image`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-image)
- [`background-origin`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-origin)
- [`background-position`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-position)
- [`background-repeat`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-repeat)
- [`background-size`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-size)
- [`border`](https://developer.mozilla.org/en-US/docs/Web/CSS/border)
- [`border-bottom`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-bottom)
- [`border-bottom-color`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-bottom-color)
- [`border-bottom-left-radius`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-bottom-left-radius)
- [`border-bottom-right-radius`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-bottom-right-radius)
- [`border-bottom-style`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-bottom-style)
- [`border-bottom-width`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-bottom-width)
- [`border-collapse`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-collapse)
- [`border-color`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-color)
- [`border-left`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-left)
- [`border-left-color`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-left-color)
- [`border-left-style`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-left-style)
- [`border-left-width`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-left-width)
- [`border-radius`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-radius)
- [`border-right`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-right)
- [`border-right-color`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-right-color)
- [`border-right-style`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-right-style)
- [`border-right-width`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-right-width)
- [`border-spacing`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-spacing)
- [`border-style`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-style)
- [`border-top`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-top)
- [`border-top-color`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-top-color)
- [`border-top-left-radius`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-top-left-radius)
- [`border-top-right-radius`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-top-right-radius)
- [`border-top-style`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-top-style)
- [`border-top-width`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-top-width)
- [`border-width`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-width)
- [`bottom`](https://developer.mozilla.org/en-US/docs/Web/CSS/bottom)
- [`box-shadow`](https://developer.mozilla.org/en-US/docs/Web/CSS/box-shadow)
- [`box-sizing`](https://developer.mozilla.org/en-US/docs/Web/CSS/box-sizing)
- [`break-after`](https://developer.mozilla.org/en-US/docs/Web/CSS/break-after)
- [`break-before`](https://developer.mozilla.org/en-US/docs/Web/CSS/break-before)
- [`break-inside`](https://developer.mozilla.org/en-US/docs/Web/CSS/break-inside)
- [`caption-side`](https://developer.mozilla.org/en-US/docs/Web/CSS/caption-side)
- [`caret-color`](https://developer.mozilla.org/en-US/docs/Web/CSS/caret-color)
- [`clear`](https://developer.mozilla.org/en-US/docs/Web/CSS/clear)
- [`color`](https://developer.mozilla.org/en-US/docs/Web/CSS/color)
- [`color-adjust`](https://developer.mozilla.org/en-US/docs/Web/CSS/color-adjust)
- [`column-count`](https://developer.mozilla.org/en-US/docs/Web/CSS/column-count)
- [`column-fill`](https://developer.mozilla.org/en-US/docs/Web/CSS/column-fill)
- [`column-gap`](https://developer.mozilla.org/en-US/docs/Web/CSS/column-gap)
- [`column-rule`](https://developer.mozilla.org/en-US/docs/Web/CSS/column-rule)
- [`column-rule-color`](https://developer.mozilla.org/en-US/docs/Web/CSS/column-rule-color)
- [`column-rule-style`](https://developer.mozilla.org/en-US/docs/Web/CSS/column-rule-style)
- [`column-rule-width`](https://developer.mozilla.org/en-US/docs/Web/CSS/column-rule-width)
- [`column-span`](https://developer.mozilla.org/en-US/docs/Web/CSS/column-span)
- [`column-width`](https://developer.mozilla.org/en-US/docs/Web/CSS/column-width)
- [`columns`](https://developer.mozilla.org/en-US/docs/Web/CSS/columns)
- [`counter-increment`](https://developer.mozilla.org/en-US/docs/Web/CSS/counter-increment)
- [`counter-reset`](https://developer.mozilla.org/en-US/docs/Web/CSS/counter-reset)
- [`cursor`](https://developer.mozilla.org/en-US/docs/Web/CSS/cursor)
- [`direction`](https://developer.mozilla.org/en-US/docs/Web/CSS/direction)
- [`display`](https://developer.mozilla.org/en-US/docs/Web/CSS/display)
- `elevation`
- [`empty-cells`](https://developer.mozilla.org/en-US/docs/Web/CSS/empty-cells)
- [`filter`](https://developer.mozilla.org/en-US/docs/Web/CSS/filter)
- [`flex`](https://developer.mozilla.org/en-US/docs/Web/CSS/flex)
- [`flex-basis`](https://developer.mozilla.org/en-US/docs/Web/CSS/flex-basis)
- [`flex-direction`](https://developer.mozilla.org/en-US/docs/Web/CSS/flex-direction)
- [`flex-flow`](https://developer.mozilla.org/en-US/docs/Web/CSS/flex-flow)
- [`flex-grow`](https://developer.mozilla.org/en-US/docs/Web/CSS/flex-grow)
- [`flex-shrink`](https://developer.mozilla.org/en-US/docs/Web/CSS/flex-shrink)
- [`flex-wrap`](https://developer.mozilla.org/en-US/docs/Web/CSS/flex-wrap)
- [`float`](https://developer.mozilla.org/en-US/docs/Web/CSS/float)
- [`font`](https://developer.mozilla.org/en-US/docs/Web/CSS/font)
- [`font-family`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-family)
- [`font-feature-settings`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-feature-settings)
- [`font-kerning`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-kerning)
- [`font-size`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-size)
- [`font-size-adjust`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-size-adjust)
- [`font-stretch`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-stretch)
- [`font-style`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-style)
- [`font-synthesis`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-synthesis)
- [`font-variant`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-variant)
- [`font-variant-alternates`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-variant-alternates)
- [`font-variant-caps`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-variant-caps)
- [`font-variant-east-asian`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-variant-east-asian)
- [`font-variant-ligatures`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-variant-ligatures)
- [`font-variant-numeric`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-variant-numeric)
- [`font-variation-settings`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-variation-settings)
- [`font-weight`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-weight)
- [`gap`](https://developer.mozilla.org/en-US/docs/Web/CSS/gap)
- [`grid`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid)
- [`grid-area`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-area)
- [`grid-auto-columns`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-auto-columns)
- [`grid-auto-flow`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-auto-flow)
- [`grid-auto-rows`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-auto-rows)
- [`grid-column`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-column)
- [`grid-column-end`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-column-end)
- [`grid-column-start`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-column-start)
- [`grid-row`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-row)
- [`grid-row-end`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-row-end)
- [`grid-row-start`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-row-start)
- [`grid-template`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-template)
- [`grid-template-areas`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-template-areas)
- [`grid-template-columns`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-template-columns)
- [`grid-template-rows`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-template-rows)
- [`height`](https://developer.mozilla.org/en-US/docs/Web/CSS/height)
- [`hyphens`](https://developer.mozilla.org/en-US/docs/Web/CSS/hyphens)
- [`image-orientation`](https://developer.mozilla.org/en-US/docs/Web/CSS/image-orientation)
- `image-resolution`
- [`inline-size`](https://developer.mozilla.org/en-US/docs/Web/CSS/inline-size)
- [`isolation`](https://developer.mozilla.org/en-US/docs/Web/CSS/isolation)
- [`justify-content`](https://developer.mozilla.org/en-US/docs/Web/CSS/justify-content)
- [`justify-items`](https://developer.mozilla.org/en-US/docs/Web/CSS/justify-items)
- [`justify-self`](https://developer.mozilla.org/en-US/docs/Web/CSS/justify-self)
- [`left`](https://developer.mozilla.org/en-US/docs/Web/CSS/left)
- [`letter-spacing`](https://developer.mozilla.org/en-US/docs/Web/CSS/letter-spacing)
- [`line-break`](https://developer.mozilla.org/en-US/docs/Web/CSS/line-break)
- [`line-height`](https://developer.mozilla.org/en-US/docs/Web/CSS/line-height)
- [`list-style`](https://developer.mozilla.org/en-US/docs/Web/CSS/list-style)
- [`list-style-position`](https://developer.mozilla.org/en-US/docs/Web/CSS/list-style-position)
- [`list-style-type`](https://developer.mozilla.org/en-US/docs/Web/CSS/list-style-type)
- [`margin`](https://developer.mozilla.org/en-US/docs/Web/CSS/margin)
- [`margin-bottom`](https://developer.mozilla.org/en-US/docs/Web/CSS/margin-bottom)
- [`margin-left`](https://developer.mozilla.org/en-US/docs/Web/CSS/margin-left)
- [`margin-right`](https://developer.mozilla.org/en-US/docs/Web/CSS/margin-right)
- [`margin-top`](https://developer.mozilla.org/en-US/docs/Web/CSS/margin-top)
- [`max-height`](https://developer.mozilla.org/en-US/docs/Web/CSS/max-height)
- [`max-width`](https://developer.mozilla.org/en-US/docs/Web/CSS/max-width)
- [`min-height`](https://developer.mozilla.org/en-US/docs/Web/CSS/min-height)
- [`min-width`](https://developer.mozilla.org/en-US/docs/Web/CSS/min-width)
- [`mix-blend-mode`](https://developer.mozilla.org/en-US/docs/Web/CSS/mix-blend-mode)
- [`object-fit`](https://developer.mozilla.org/en-US/docs/Web/CSS/object-fit)
- [`object-position`](https://developer.mozilla.org/en-US/docs/Web/CSS/object-position)
- [`offset-distance`](https://developer.mozilla.org/en-US/docs/Web/CSS/offset-distance)
- [`opacity`](https://developer.mozilla.org/en-US/docs/Web/CSS/opacity)
- [`order`](https://developer.mozilla.org/en-US/docs/Web/CSS/order)
- [`outline`](https://developer.mozilla.org/en-US/docs/Web/CSS/outline)
- [`outline-color`](https://developer.mozilla.org/en-US/docs/Web/CSS/outline-color)
- [`outline-offset`](https://developer.mozilla.org/en-US/docs/Web/CSS/outline-offset)
- [`outline-style`](https://developer.mozilla.org/en-US/docs/Web/CSS/outline-style)
- [`outline-width`](https://developer.mozilla.org/en-US/docs/Web/CSS/outline-width)
- [`overflow`](https://developer.mozilla.org/en-US/docs/Web/CSS/overflow)
- [`overflow-x`](https://developer.mozilla.org/en-US/docs/Web/CSS/overflow-x)
- [`overflow-y`](https://developer.mozilla.org/en-US/docs/Web/CSS/overflow-y)
- [`overflow-wrap`](https://developer.mozilla.org/en-US/docs/Web/CSS/overflow-wrap)
- [`padding`](https://developer.mozilla.org/en-US/docs/Web/CSS/padding)
- [`padding-bottom`](https://developer.mozilla.org/en-US/docs/Web/CSS/padding-bottom)
- [`padding-left`](https://developer.mozilla.org/en-US/docs/Web/CSS/padding-left)
- [`padding-right`](https://developer.mozilla.org/en-US/docs/Web/CSS/padding-right)
- [`padding-top`](https://developer.mozilla.org/en-US/docs/Web/CSS/padding-top)
- `pause`
- `pause-after`
- `pause-before`
- [`perspective`](https://developer.mozilla.org/en-US/docs/Web/CSS/perspective)
- [`perspective-origin`](https://developer.mozilla.org/en-US/docs/Web/CSS/perspective-origin)
- `pitch`
- `pitch-range`
- [`place-items`](https://developer.mozilla.org/en-US/docs/Web/CSS/place-items)
- [`position`](https://developer.mozilla.org/en-US/docs/Web/CSS/position)
- [`quotes`](https://developer.mozilla.org/en-US/docs/Web/CSS/quotes)
- [`resize`](https://developer.mozilla.org/en-US/docs/Web/CSS/resize)
- `richness`
- [`right`](https://developer.mozilla.org/en-US/docs/Web/CSS/right)
- [`row-gap`](https://developer.mozilla.org/en-US/docs/Web/CSS/row-gap)
- `speak`
- `speak-header`
- `speak-numeral`
- `speak-punctuation`
- `speech-rate`
- `stress`
- [`table-layout`](https://developer.mozilla.org/en-US/docs/Web/CSS/table-layout)
- [`text-align`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-align)
- [`text-align-last`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-align-last)
- [`text-combine-upright`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-combine-upright)
- [`text-decoration`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-decoration)
- [`text-decoration-color`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-decoration-color)
- [`text-decoration-line`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-decoration-line)
- [`text-decoration-skip`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-decoration-skip)
- [`text-decoration-style`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-decoration-style)
- [`text-emphasis`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-emphasis)
- [`text-emphasis-color`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-emphasis-color)
- [`text-emphasis-position`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-emphasis-position)
- [`text-emphasis-style`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-emphasis-style)
- [`text-indent`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-indent)
- [`text-justify`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-justify)
- [`text-orientation`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-orientation)
- [`text-overflow`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-overflow)
- [`text-shadow`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-shadow)
- [`text-transform`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-transform)
- [`text-underline-position`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-underline-position)
- [`top`](https://developer.mozilla.org/en-US/docs/Web/CSS/top)
- [`transform`](https://developer.mozilla.org/en-US/docs/Web/CSS/transform)
- [`transform-box`](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-box)
- [`transform-origin`](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-origin)
- [`transform-style`](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-style)
- [`transition`](https://developer.mozilla.org/en-US/docs/Web/CSS/transition)
- [`transition-delay`](https://developer.mozilla.org/en-US/docs/Web/CSS/transition-delay)
- [`transition-duration`](https://developer.mozilla.org/en-US/docs/Web/CSS/transition-duration)
- [`transition-property`](https://developer.mozilla.org/en-US/docs/Web/CSS/transition-property)
- [`transition-timing-function`](https://developer.mozilla.org/en-US/docs/Web/CSS/transition-timing-function)
- [`unicode-bidi`](https://developer.mozilla.org/en-US/docs/Web/CSS/unicode-bidi)
- [`vertical-align`](https://developer.mozilla.org/en-US/docs/Web/CSS/vertical-align)
- [`visibility`](https://developer.mozilla.org/en-US/docs/Web/CSS/visibility)
- `voice-family`
- [`white-space`](https://developer.mozilla.org/en-US/docs/Web/CSS/white-space)
- [`width`](https://developer.mozilla.org/en-US/docs/Web/CSS/width)
- [`word-break`](https://developer.mozilla.org/en-US/docs/Web/CSS/word-break)
- [`word-spacing`](https://developer.mozilla.org/en-US/docs/Web/CSS/word-spacing)
- [`word-wrap`](https://developer.mozilla.org/en-US/docs/Web/CSS/word-wrap)
- [`writing-mode`](https://developer.mozilla.org/en-US/docs/Web/CSS/writing-mode)
- [`z-index`](https://developer.mozilla.org/en-US/docs/Web/CSS/z-index)

### 추가 제한 사항 <a name="additional-restrictions"></a>

다음 CSS 속성에는 추가 제한 사항이 있습니다.

| 속성                                                                        | 제한 사항                                                                                   |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| [`cursor`](https://developer.mozilla.org/en-US/docs/Web/CSS/cursor)         | 허용되는 값은 `pointer` 및 `initial`뿐입니다.                                               |
| [`filter`](https://developer.mozilla.org/en-US/docs/Web/CSS/filter)         | `url()`은 허용되지 않습니다.                                                                |
| [`transition`](https://developer.mozilla.org/en-US/docs/Web/CSS/transition) | `opacity`, `transform`, `visibility` 및 `offset-distance`에만 애니메이션 적용이 가능합니다. |
| [`visibility`](https://developer.mozilla.org/en-US/docs/Web/CSS/visibility) | 허용되는 값은 `hidden`, `visible` 및 `initial`뿐입니다.                                     |
| [`z-index`](https://developer.mozilla.org/en-US/docs/Web/CSS/z-index)       | -100~100 사이의 값만 허용됩니다.                                                            |

## @-규칙 <a name="at-rules"></a>

현재 지원되는 [@-규칙](https://developer.mozilla.org/en-US/docs/Web/CSS/At-rule)은 `@media`뿐입니다. 자세한 내용은 [미디어 기능](#media-features)을 참조하세요.

### 사용자 지정 글꼴(`@font-face`) <a name="custom-fonts-font-face"></a>

이메일용 AMP에서 사용자 지정 글꼴은 지원되지 **않습니다**.

## 미디어 기능 <a name="media-features"></a>

`@media` 쿼리를 통한 조건부 적용 규칙에 지원되는 [미디어 기능](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries#Media_features) 목록입니다.

- [`device-width`](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/device-width)
  - `max-device-width`
  - `min-device-width`
- [`hover`](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/hover)
- [`orientation`](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/orientation)
- [`pointer`](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/pointer)
- [`resolution`](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/resolution)
  - `max-resolution`
  - `min-resolution`
- [`width`](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/width)
  - `max-width`
  - `min-width`
