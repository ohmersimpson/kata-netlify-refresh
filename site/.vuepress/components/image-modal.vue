<template>
    <div>
		<a href="#" @click.prevent="isImageModalActive = true" >
			<img :src="imgurl" :alt="imgurl" />
		</a>
        <b-modal :active.sync="isImageModalActive" :width="1080">
            <p class="image is-4by3">
				<a href="#">
					<img :src="imgurl">
				</a>
            </p>
        </b-modal>		
    </div>
</template>
	

<script>

	export default {
		/**
		 * The name of the component.
		 *
		 * @type {Strng}
		 */
		name: 'ImageModal',

		props: 
			['imgurl']
		,
		data() {
            return {
                isImageModalActive: false,
            }
        },

		

	}
</script>
