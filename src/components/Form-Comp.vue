<template>
    <h2>Text Input</h2>
    <input v-model="text">{{text}}
    <h2>Checkbox</h2>
    <input type="checkbox" id="checkbox" v-model="checked" >
    <label for="checkbox">checked:{{checked}}</label>
    <h2>Multi Checkbox</h2>
    <input type="checkbox" id="Cheslyn" v-model="checkedNames" value="Cheslyn"> 
    <label for="Cheslyn">Cheslyn</label>
    <input type="checkbox" id="Luke" v-model="checkedNames" value="Luke">
    <label for="Luke">Luke</label>
    <p>checked: 
        <pre>{{checkedNames}}</pre>
    </p>
    <h2>Radio</h2>
    <input type="radio" id="one" value="One" v-model="picked">
    <label for="one">One</label>
    <br>
    <input type="radio" id="two" value="Two" v-model="picked">
    <label for="two">Two</label>
    <br>
    <span>Picked: {{picked}}</span>
    <h2>Multi Select</h2>
    <select v-model="multiSelected" multiple style="width:100px">
        <option value="A">A</option>
        <option value="B">B</option>
        <option value="C">C</option>
    </select><br>
    <span>Selected: {{multiSelected}}</span>
    
</template> 

<script>
export default {
    data(){
        return {text:'', 
                checked: true,
                checkedNames: ['Cheslyn'],
                picked: 'One',
                multiSelected: ['A']
                }
    }
}
</script>