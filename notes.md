notes.md

<div id="recipe">
  {{name}}
  {{each ingredient}}
    {{>recipeDetailsPartial}}
{{/each}}
<a href="{{url}}" onclick="displayEditForm()">Edit Recipe</a> -->
</div>
</script>

<script id="recipe-details-partial" type="text/x-handlebars-template">
{{#each ingredient}}
  {{displayIngredient(this)}}
{{/each}}
</script>




//form

<form id='recipe-form' onSubmit="createRecipe()">
  <!--name, description, five ingredients-->
  Name:         <input type="text" id="name"><br>
  Description:  <input type="text" name="description"><br>
  Ingredient:   <input type="text" name="ingredients"><br>
  Ingredient:   <input type="text" name="ingredients"><br>
  Ingredient:   <input type="text" name="ingredients"><br>
  Ingredient:   <input type="text" name="ingredients"><br>
  Ingredient:   <input type="text" name="ingredients"><br>
  Ingredient:   <input type="text" name="ingredients"><br>
  <input type="submit">
</form>
