<script>
    let installationSteps = [
        "Install Node.js",
        "Run `npx sv create lab10c`",
        "Install dependencies with `npm install`",
        "Start the development server with `npm run dev -- --open`"
    ];

    let challenges = [
        {
            issue: "Understanding SvelteKit as well as how development frameworks work.",
            solution: "Watched tutorials on YouTube as well as following the official documentation while working on this project."
        },
        {
            issue: "Configuring hosting on Vercel.",
            solution: "Read Vercel's deployment guide and used the Vercel CLI."
        }
    ];
</script>

<style>
    body {
        font-family: Arial, sans-serif;
        line-height: 1.6;
    }

    .container {
        max-width: 800px;
        margin: auto;
        padding: 20px;
    }

    h1, h2 {
        color: black;
    }

    .code {
        background-color: #dfdfdf;
        padding: 10px;
        margin-bottom: 20px;
    }

    ul {
        list-style-type: disc;
        padding-left: 20px;
    }

    li {
        margin-bottom: 10px;
    }
</style>

    <div class="container">
        <h1>Building This Webpage with SvelteKit</h1>
        <p>This webpage was built using the SvelteKit development framework.</p>

        <h2>Installation Steps</h2>
        <ul>
            {#each installationSteps as step}
                <li>{step}</li>
            {/each}
        </ul>

        <h2>Challenges and Solutions</h2>
        <div>
            {#each challenges as { issue, solution }}
                <div class="code">
                    <strong>Issue:</strong> {issue} <br />
                    <strong>Solution:</strong> {solution}
                </div>
            {/each}
        </div>
    </div>
