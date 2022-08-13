# Add new ingredient

ThymeSave is only as powerful as the ingredients we know and can detect.

## Walk through

1. Create new ingredient
    1. The list of all ingredients is maintained in `projects/thymesave/ingredients/src/lib/ingredients.ts`
    2. Check if the ingredient you want to add has already an appropriate category, if
       not [add one](./add_ingredient_category.md).
2. Now ThymeSave knows about the ingredient, which is great!
3. Let's go on and add translations, so we can match the ingredient information to actual localized variants.
    1. Each language has its own folder and ingredient translations maintained
       in `projects/thymesave/translations/src/resources/<language_code>/ingredients.ts`
    2. Add a singular and (if applicable pluralized translation) format is (first element: singular, second element:
       plural)
    3. Make sure to add at least the english version of the ingredient
4. Make sure you added the keys in alphabetical correct order, when linting passes you can create your PR
