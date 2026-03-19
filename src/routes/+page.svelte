<script lang="ts">
    import profilePic from "$lib/assets/profile-pic-alt.svg";
</script>

<div class="container">
    <div class="main-profile-container">
        <h1>Felix Andersen</h1>
        <p>Software Engineer</p>
        <small>Work in progress...</small>
    </div>
</div>

<style>
    .container {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        background-color: rgba(0, 0, 0, 0.025);
    }

    .main-profile-container {
        font-family: "Roboto", monospace;
        background-color: rgba(0, 0, 0, 0.05);
        color: rgba(0, 0, 0, 0.7);
        width: 25%;
        border-radius: 0.5em;
        padding: 0.25em 0 1em 1em;
        box-shadow: 0 0 15px 5px rgba(0, 0, 0, 0.1);
    }
</style>
