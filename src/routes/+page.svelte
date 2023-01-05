<script lang="ts" context="module">

</script>

<script lang="ts">
    const education = [{
        name: "foo bar",
        from: "Sept 2008",
        to: "Jan 2010"
    }]

    const experience = [{
        name: "Freelance Translator",
        descriptions: [
            'Historical, journal, literature translation (Mandarin-English, Cantonese-English)',
            'Transcription (Mandarin-English,Cantonese-English)',
            'Subtitling (Mandarin-English,Cantonese-English)',
            'Company: Elite Asia, TED, SOAS University of London'
        ],
        from: "Sep 2022",
        to: "Present"
    }]
</script>

<section>
    <h2>Personal profile</h2>
    <p>A highly positive, enthusiastic and adaptive Chinese-English translator who has just finished her masters degree. A person who loves challenges and learning new things, being able to work under pressure. A good communicator with people as well as building good relationships. A person who loves sharing knowledge with others and has previous experience in tutoring, and cooperating with colleagues and members.</p>
</section>

<section id="visa">
    <h2>Visa Status</h2>
    <p>Eligible to work full-time in the U.K. under the BNO Visa scheme without sponsorship.</p>
</section>

<section id="education">
    <h2>Education</h2>
    <ul>
        {#each education as { name, from, to}}
        <li>
            <div class="header">
                <p>{name}</p>
                <span>{from}-{to}</span>
            </div>
        </li>
        {/each}
    </ul>
</section>

<section>
    <h2>Experience</h2>
    <ul>
        {#each experience as { name, descriptions, from, to }}
        <li>
            <div class="experience-header">
                <p>{name}</p>
                <span>{from}-{to}</span>
            </div>
            <ul>
                {#each descriptions as d}
                <li>{d}</li>
                {/each}
            </ul>
        </li>
        {/each}       
    </ul>
</section>

<style>
    section {
        margin-bottom: 1rem;
    }
</style>