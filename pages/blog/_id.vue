<template>
    <div>
        <h2>blog detail</h2>
        <p>これは、{{ $route.params.id }}のエントリーです。</p>
    </div>
</template>

<script>
export default {
    validate({ params }){
        // 数字のみ受付
        return /^\d+$/.test(params.id);
    }
}
</script>