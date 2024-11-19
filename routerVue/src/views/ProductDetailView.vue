<template>
    <div>
        <h2>Product Detail</h2>
        <p><span>ID:</span> {{ $route.params.id }}</p>
        <p><span>Name:</span> {{ $route.params.name }}</p>
        <p><span>Description:</span> {{ $route.params.description }}</p>
    </div>
</template>

<style scoped>

div h2, p {
    padding: 0.5rem;
}

span {
    font-weight: bold;
}

</style>