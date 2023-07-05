<template>
    <section>
        <div>
            <h3>
                {{ fullName }}
                <base-badge :type="role" :caption="role.toUpperCase()"></base-badge>
            </h3>
        </div>

        <p>{{ infoText }}</p>
    </section>
</template>

<script>
    export default {
        props: ['fullName', 'infoText', 'role'],
    }
</script>