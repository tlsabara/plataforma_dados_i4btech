<script setup>

import { reactive} from "vue";

const titleClass = reactive(() => {
    return ['me-auto', `text-${this.variant}`? this.variant !== '' : '']
})

defineProps({
    variant: {
        type: String,
        default: '',
    }
})

</script>

<template>
    <main>
        <div class="position-absolute top-0 end-0 mt-5 mx-5 p-0 toast show text-dark" role="alert"
             aria-live="assertive" aria-atomic="true">
            <div class="toast-header">
                <strong :class="titleClass">
                    <slot name="title"></slot>
                </strong>
                <small>
                    <slot name="time"></slot>
                </small>
                <button type="button" class="btn-close ms-2 mb-1" data-bs-dismiss="toast" aria-label="Close">
                    <span aria-hidden="true"></span>
                </button>
            </div>
            <div class="toast-body">
                <slot name="message"></slot>
            </div>
        </div>
    </main>
</template>

<style scoped>

</style>