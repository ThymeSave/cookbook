# Add new ingredient category

Ingredient categories are used to group ingredients together, making it easier to organize and search.

For most ingredients you will already find an appropriate category, but sometimes a new one might be required.

## Walk through

1. Add the category
    1. Open `projects/thymesave/ingredients/src/lib/ingredients.ts`
    2. At the top of the file you can see different categories, grouped together, and joined to a single batch of
       categories
    3. Find the appropriate place and add your category
2. Now ThymeSave knows about the category, which is great!
3. Let's go on and add translations, so it can be properly localized and displayed to users
    1. Each language has its own folder and ingredient category translations maintained
       in `projects/thymesave/translations/src/resources/<language_code>/ingredientCategories.ts`
    2. Add a new key for your new category containing the localized name
    3. Make sure to add at least the english version of the ingredient category
4. Make sure you added the keys in alphabetical correct order, when linting passes you can create your PR
