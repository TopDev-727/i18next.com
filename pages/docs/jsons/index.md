---
title: JSON Structure
order: 6
---

<a name="v3"></a>
### [i18next JSON v3](#v3)

```json
{
  "key": "value",
  "keyDeep": {
    "inner": "value"
  },
  "keyNesting": "reuse $t{keyDeep.inner}",
  "keyInterpolate": "replace this {{value}}",
  "keyInterpolateUnescaped": "replace this {{- value}}",
  "keyInterpolateWithFormatting": "replace this {{value, format}}",
  "keyContext_male": "the male variant",
  "keyContext_female": "the female variant",
  "keyPluralSimple": "the singular",
  "keyPluralSimple_plural": "the plural",
  "keyPluralMultipleEgArabic_0": "the plural form 0",
  "keyPluralMultipleEgArabic_1": "the plural form 1",
  "keyPluralMultipleEgArabic_2": "the plural form 2",
  "keyPluralMultipleEgArabic_3": "the plural form 3",
  "keyPluralMultipleEgArabic_4": "the plural form 4",
  "keyPluralMultipleEgArabic_5": "the plural form 5"
}
```

This are the defaults. Nesting and Interpolation formats are configurable.

The only difference to [v2](#v2) are the plural suffixes for languages with multiple plural forms.

<a name="v2"></a>
### [i18next JSON v2](#v2)

enabled by:

```js
i18next.init({
  compatibilityJSON: 'v2'
});
```

formats:

```json
{
  "key": "value",
  "keyDeep": {
    "inner": "value"
  },
  "keyNesting": "reuse $t{keyDeep.inner}",
  "keyInterpolate": "replace this {{value}}",
  "keyInterpolateUnescaped": "replace this {{- value}}",
  "keyContext_male": "the male variant",
  "keyContext_female": "the female variant",
  "keyPluralSimple": "the singular",
  "keyPluralSimple_plural": "the plural",
  "keyPluralMultipleEgArabic_0": "the plural form 0",
  "keyPluralMultipleEgArabic_1": "the plural form 1",
  "keyPluralMultipleEgArabic_2": "the plural form 2",
  "keyPluralMultipleEgArabic_3": "the plural form 3",
  "keyPluralMultipleEgArabic_11": "the plural form 4",
  "keyPluralMultipleEgArabic_100": "the plural form 5"
}
```

This are the defaults. Nesting and Interpolation formats are configurable.

<a name="v1"></a>
### [i18next JSON v1](#v1)

enabled by:

```js
i18next.init({
  compatibilityJSON: 'v1'
});
```

formats:

```json
{
  "key": "value",
  "keyDeep": {
    "inner": "value"
  },
  "keyNesting": "reuse $t{keyDeep.inner}",
  "keyInterpolate": "replace this __value__",
  "keyInterpolateUnescaped": "replace this __valueHTML__",
  "keyContext_male": "the male variant",
  "keyContext_female": "the female variant",
  "keyPluralSimple": "the singular",
  "keyPluralSimple_plural": "the plural",
  "keyPluralMultipleEgArabic": "the plural form 0",
  "keyPluralMultipleEgArabic_plural_1": "the plural form 1",
  "keyPluralMultipleEgArabic_plural_2": "the plural form 2",
  "keyPluralMultipleEgArabic_plural_3": "the plural form 3",
  "keyPluralMultipleEgArabic_plural_11": "the plural form 4",
  "keyPluralMultipleEgArabic_plural_100": "the plural form 5"
}
```

This are the defaults. Nesting and Interpolation formats are configurable.
