<script>
import { objectToString } from '@vue/shared';

export default {
    name: "CardGenerator",
    // attraverso il props richiamo le informazione da inserire nella card dal padre Listcard che le contiene
    props: {
        info: Object
    }
}
</script>

<template>
    <!-- creo la card -->
    <div class="gen_card">
        <div class="slot_img_card">
            <img :src="info.thumb" :alt="info.series">
        </div>
        <h4><span>Titolo:</span> {{ info.series }}</h4>
        <span><strong>Prezzo:</strong> {{ info.price }}</span>
        <br>
        <span><strong>Categoria:</strong> {{ info.type }}</span>
    </div>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;

.gen_card {
    width: calc(100% / 6);
    padding: 10px;

    .slot_img_card {
        margin-bottom: 10px;
    }

    span {
        color: $secondaryColor;
    }
}
</style>