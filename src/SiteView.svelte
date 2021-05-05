<script lang="ts">
  import { Site } from "./types";
  export let site: Site;
</script>

<main>
  <div class="card m-4">
    <div class="card-header">
      <div class="card-header-title "><p class="title is-4">{site.title}</p></div>
      <div class="card-header-icon" aria-label="more options">
        <a href={site.url} target="_blank">
          <span class="icon">
            <i class="fas fa-external-link-alt" aria-hidden="true"></i>
          </span>
        </a>
      </div>
    </div>
    <div class="card-content">
      <p class="subtitle is-6">URL: <a href={site.url} target="_blank">{site.url}</a></p>
      <p>{site.description}</p>
    </div>
  </div>
</main>

<style>
</style>