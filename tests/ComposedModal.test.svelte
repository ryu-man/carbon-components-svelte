<script lang="ts">
  import {
    ComposedModal,
    ModalHeader,
    ModalBody,
    ModalFooter,
    Checkbox,
  } from "../types";

  let checked = false;
</script>

<ComposedModal open>
  <ModalHeader title="Confirm changes" />
  <ModalBody hasForm>
    <Checkbox labelText="I have reviewed the changes" bind:checked />
  </ModalBody>
  <ModalFooter primaryButtonText="Proceed" primaryButtonDisabled="{!checked}" />
</ComposedModal>
