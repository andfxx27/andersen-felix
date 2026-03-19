<script lang="ts">
    import { base } from "$app/paths";
    import IconsLinkedin from "~icons/entypo-social/linkedin-with-circle";
    import IconsGithub from "~icons/entypo-social/github-with-circle";
    import IconsTwitter from "~icons/entypo-social/twitter-with-circle";

    // Using Svelte 5 runes correctly
    let year = $state(new Date().getFullYear());
</script>

<div class="container">
    <main class="main-profile-container">
        <h1>Felix Andersen</h1>
        <p class="title">Software Engineer</p>

        <div class="bio-container">
            <p class="quick-description">
                Currently working at one of the largest private banks in
                Indonesia.
                <small class="disclaimer"
                    >Opinions are my own and do not represent my employer.</small
                >
            </p>

            <p class="quick-description">
                Exploring more about full-stack application development with a
                focus on backend engineering.
            </p>

            <p class="quick-description">Feel free to connect with me!</p>
        </div>

        <nav class="socials-container" aria-label="Social media links">
            <a
                href="https://www.linkedin.com/in/felix-andersen-84276b185/"
                target="_blank"
                rel="noopener noreferrer"
                aria-label="LinkedIn"
            >
                <IconsLinkedin />
            </a>
            <a
                href="https://github.com/andfxx27"
                target="_blank"
                rel="noopener noreferrer"
                aria-label="GitHub"
            >
                <IconsGithub />
            </a>
            <a
                href="https://twitter.com/And_Fxx"
                target="_blank"
                rel="noopener noreferrer"
                aria-label="Twitter"
            >
                <IconsTwitter />
            </a>
        </nav>

        <footer>
            <small>&copy; {year} Felix Andersen</small>
        </footer>
    </main>
</div>

<style>
    :global(body) {
        margin: 0;
        padding: 0;
    }

    a,
    a:link,
    a:visited {
        color: inherit;
        text-decoration: none;
    }

    .bio-container {
        margin-bottom: 1.5rem;
    }

    .quick-description {
        display: block;
        font-size: 0.9rem;
        line-height: 1.6;
        margin-bottom: 0.75rem;
        color: #555;
    }

    .disclaimer {
        display: block;
        font-size: 0.75rem;
        color: #888;
        font-style: italic;
        margin-top: 0.25rem;
    }

    .container {
        display: flex;
        justify-content: center;
        align-items: center;
        min-height: 100vh;
        background-color: #f8f9fa; /* More solid background */
    }

    .main-profile-container {
        font-family: "Roboto", sans-serif; /* Roboto is usually sans-serif, not monospace */
        background-color: white;
        color: #333;

        /* Better responsive width */
        width: 90%;
        max-width: 400px;

        border-radius: 12px;
        padding: 2rem;
        box-shadow: 0 10px 25px rgba(0, 0, 0, 0.05);
        text-align: left;
    }

    h1 {
        margin: 0;
        font-size: 1.5rem;
    }

    .title {
        margin: 0.2rem 0 1rem 0;
        font-weight: 500;
        color: #666;
    }

    .quick-description {
        display: block;
        line-height: 1.5;
        margin-bottom: 1.5rem;
        color: #777;
    }

    .socials-container {
        display: flex;
        align-items: center;
        gap: 1rem;
        margin-bottom: 1.5rem;
    }

    /* Hover effects for social icons */
    .socials-container a {
        font-size: 1.5rem;
        transition:
            transform 0.2s ease,
            color 0.2s ease;
        display: flex;
        opacity: 0.8;
    }

    .socials-container a:hover {
        transform: translateY(-3px);
        opacity: 1;
        color: #000;
    }

    footer {
        border-top: 1px solid #eee;
        padding-top: 1rem;
    }
</style>
