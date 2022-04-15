<script context="module">
  export const load = ({ error, status }) => {
    return {
      props: {
        error,
        status,
      },
    };
  };
</script>

<script lang="ts">
  import type { IError } from "src/types/error";

  export let error: IError;
  export let status: number;
</script>

<h1>{error.name} {status}</h1>
<p>{error.message}</p>
