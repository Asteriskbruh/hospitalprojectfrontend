<script context="module">
    export async function load({fetch,params}) {
        const res = await fetch('http://localhost:8080/home/'+params.id);
        const data = await res.json();
        if(res.ok){
            return {
                props : {Data : data}
            }
        }
    }
    

</script>

<h1>job done !!!</h1>