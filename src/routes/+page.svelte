<script lang="ts" context="module">

</script>

<script lang="ts">

    const education = [{
        name: "foo bar",
        from: "Sept 2008",
        to: "Jan 2010"
    }]

    const experience = [
        {
        name: "Freelance Translator",
        descriptions: [
            'Historical, journal, literature translation (Mandarin-English, Cantonese-English)',
            'Transcription (Mandarin-English,Cantonese-English)',
            'Subtitling (Mandarin-English,Cantonese-English)',
            'Company: Elite Asia, TED, SOAS University of London'
        ],
        from: "Sep 2022",
        to: "Present"
        }, {
            name: "Music Teacher (Part-time)",
        descriptions: [
            'Taught electrical keyboard classes (Soundsteps and Trinity grade)',
            'Covered teaching when required',
            'Carried out Soundsteps Music School internal examinations'
        ],
        from: "Apr 2022",
        to: "Oct 2022",
        company: "Howard Music School LTD (UK)"
        }, {
            name: "Teaching Assistant in Bilingual Class",
        descriptions: [
            'Assisted to plan and prepare programme materials',
            'Assisted instructors to ensure class operation smoothly',
            'Provided proper care and supervision to participants',
            'Facilitated a fun and safe learning environment for participants',
            'Assisted back office to prepare documents such as reports, worksheets, etc.'
        ],
        from: "Jan 2020",
        to: "Aug 2021",
        company: "Stamford American School Hong Kong"
        }, {
            name: "Support and Director",
        descriptions: [
                'Planned and prepared programme materials for Art & Design class',
                'Explored a variety of interactive drama and art activities'
        ],
        from: "Jun 2021",
        to: "Jul 2021",
        company: "Camp Asia Hong Kong"
        }
    ]
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
    <ul class="exp-list">
        {#each experience as { name, descriptions, from, to }}
        <li>
            <div class="experience-header">
                <h3>{name}</h3>
                <span>{from}-{to}</span>
            </div>
            <ul class="desc-list">
                {#each descriptions as d}
                <li>{d}</li>
                {/each}
            </ul>
        </li>
        {/each}       
    </ul>
</section>

<style lang="scss">
    section {
        margin-bottom: 1rem;
    }

    .exp-list {
        display: flex;
        row-gap: 1rem;
        flex-direction: column;

        .experience-header {
            margin-bottom: 0.5rem;
        }
    }

    .desc-list {
        display: flex;
        row-gap: 0.5rem;
        flex-direction: column;
        list-style: disc inside;
    }
</style>