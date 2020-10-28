<script>
    import Keyboard from 'simple-keyboard'

    let keyboard = new Keyboard({
        onChange: input => onChange(input),
        onKeyPress: button => onKeyPress(button)
    });

    function onChange(input){
        document.querySelector(".input").value = input;
        console.log("Input changed", input);
    }

    function onKeyPress(button){
        console.log("Button pressed", button);
    }
</script>


<input class="input" type="text" value="foo bar"/>
<div class="simple-keyboard"></div>


<style>
    @import 'simple-keyboard/build/css/index.css';
</style>

