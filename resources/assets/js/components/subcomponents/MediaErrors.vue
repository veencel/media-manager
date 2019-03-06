<template>
  <div
    class="modal-errors"
    transition="expand">
    <ul>
      <li
        v-for="error in errors"
        :key="error">{{ error }}</li>
    </ul>
  </div>
</template>

<script>
export default {
	props: {
		errors : {
			default: function(){
			    return [];
			},
			type: Array
		}
	}
};
</script>
