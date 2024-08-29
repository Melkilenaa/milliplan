<script lang="ts">
  import PostItem from "./PostItem.svelte";

  let posts = [
    {
      name: "Post 1",
      content:
        "This is the content of post 1. This is the content of post 1. This is the content of post 1. This is the content of post 1. This is the content of post 1. This is the content of post 1",
      date: "2021-09-01",
      summary: "This is a summary of post 1",
    },
    {
      name: "Post 2",
      content:
        "This is the content of post 1. This is the content of post 1. This is the content of post 1. This is the content of post 1. This is the content of post 1. This is the content of post 1",
      date: "2021-09-01",
      summary: "This is a summary of post 2",
    },
    {
      name: "Post 3",
      content:
        "This is the content of post 1. This is the content of post 1. This is the content of post 1. This is the content of post 1. This is the content of post 1. This is the content of post 1",
      date: "2021-09-01",
      summary: "This is a summary of post 3",
    },
    {
      name: "Post 4",
      content:
        "This is the content of post 1. This is the content of post 1. This is the content of post 1. This is the content of post 1. This is the content of post 1. This is the content of post 1",
      date: "2021-09-01",
      summary: "This is a summary of post 4",
    },
  ];
</script>

<h1>Blog</h1>

{#each posts as post (post.name)}
  <a href="/post/{post.name}" class="text-white">
    <PostItem {post} />
  </a>
{/each}
