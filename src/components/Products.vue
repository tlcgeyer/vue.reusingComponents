<template> <!--vbase to get the full layout-->
    <div>
        <!--why do we use components? 
        to access it across the page.  ALso make use of uppercase when naming a component.
    
        If there is data that is on the parent and you want to pass it to the child, make use of 'props'. 
    
    
    They can be created using an object or an array.

calling a component is like calling a function-->
        <h2>Child component</h2>
        <p>{{ greetings }} </p>

    </div>
</template>

<script>
    export default {
    name: 'ProductComp', //overwriting the name of the file to avoid the multi-word error 

    
    props: ['greetings'],

    }
</script>

<style scoped> /* only styles the elements in the current component */

</style>