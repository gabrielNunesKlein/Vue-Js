<template>
    <div>
        <button @click="$emit('mudarImagem')">Trocar Imagem</button>
    </div>
</template>

<script>
export default {
    name: "TrocaImagem",
    emitis: ["mudarImagem"]
}
</script>
