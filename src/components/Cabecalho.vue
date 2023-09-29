<script setup>
    const props = defineProps(['tarefasPendentes']);
</script>

<template>
    <header class="bg-light p-5 mt-4 mb-4">
        <h1>Minhas tarefas</h1>
        <p v-if="props.tarefasPendentes > 0">
            Você possui {{ props.tarefasPendentes }} tarefas pendentes.
        </p>
    </header>
</template>