<script lang="ts">
    import type { Post } from "./types";

    export let post: Post;
</script>

<div class="flex flex-col">
    <h1 class="text-lg font-bold">{post.name}</h1>
    <p class="text-gray-800 text-sm">{post.date}</p>

    <div>{post.content}</div>
</div>