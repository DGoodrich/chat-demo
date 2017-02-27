<template lang="html">
    <div class="chat-message">
        <p>{{ message.message }}</p>
        <small>{{ message.user.name }}</small>
        <small class="online" v-if="status.find(x => x.name === message.user.name)">- Online</small>
        <small class="offline" v-else>- Offline</small>

    </div>
</template>

<script>
    export default {
        props: ['message', 'status']
    }
</script>

<style lang="css">
    .chat-message {
        padding: 1rem;
    }
    .chat-message > p {
        margin-bottom: .5rem;
    }
    .chat-message .online {
        color: #00af0b;
    }
    .chat-message .offline {
        color: rgba(150, 160, 162, 0.76);
    }
</style>