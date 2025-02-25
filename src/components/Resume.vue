<template>
  <div class="container" :style="{ backgroundImage: `url(${parchment})` }">
    <div class="resume-wrapper">
      <header class="resume-header">
        <h1>DAVID CONRAD</h1>
        <p>Louisville, KY</p>
        <div class="contact-info">
          <span>david.scott.conrad@gmail.com</span>
          <span class="separator">|</span>
          <span>502-381-3806</span>
          <span class="separator">|</span>
          <a target="_blank" href="https://www.linkedin.com/in/david-scott-conrad/" class="link"
            >LinkedIn</a
          >
          <span class="separator">|</span>
          <a target="_blank" href="https://github.com/davidscottconrad" class="link">Github</a>
          <span class="separator">|</span>
          <a target="_blank" href="/" class="link">Portfolio</a>
        </div>
        <h2 class="job-title">FULL STACK SOFTWARE ENGINEER - 4+ YOE</h2>
      </header>

      <section class="experience-section">
        <div class="job">
          <div class="job-header">
            <h3>AHEAD / CDI</h3>
            <div class="job-location">
              <span>Chicago, IL and NY, NY (Remote)</span>
              <span>Sep 2022-Present</span>
            </div>
          </div>
          <p class="job-title-inner">IT Services and IT Consulting</p>
          <p class="job-title-inner">Full Stack Software Engineer</p>
          <ul>
            <li>Lead front end modernization of a four year old client portal.</li>
            <li>
              Created Google Maps API to validate addresses across 1 billion dollars of sales, three
              salesforce instances, our client portal database, and new incoming addresses. API
              prevents duplicate customer sites, increasing data accuracy
            </li>
            <li>
              Developed comprehensive dashboards using Servicenow, Logicmonitor, and Backup Radar
              APIs, providing customers with visibility into their services and enabling them to
              monitor their usage to reducing inquiries.
            </li>
            <li>
              Integrated HashiCorp Vault into the codebase for secure secrets management,
              collaborating with experienced DevOps engineers, which contributed to successful and
              reliable production deployments.
            </li>
          </ul>
        </div>

        <div class="job">
          <div class="job-header">
            <h3>Florida SouthWestern State College</h3>
            <div class="job-location">
              <span>Fort Myers, FL</span>
              <span>Nov 2020-Sep 2022</span>
            </div>
          </div>
          <p class="job-title-inner">Full Stack Software Engineer</p>
          <ul>
            <li>
              Modernized the Schedule Search functionality on Class Schedule Search used by 15,000
              students each semester.
              <a target="_blank" href="https://www.fsw.edu/academics/schedule_search" class="link"
                >Class Schedule Search</a
              >
            </li>
            <li>
              Maintained and updated fsw.edu in partnership with cross-functional teams, ensuring
              the site remained current and informative for students.
            </li>
          </ul>
        </div>

        <div class="job">
          <div class="job-header">
            <h3>Ethicon Inc</h3>
            <div class="job-location">
              <span>Cornelia, GA</span>
              <span>2015-2016</span>
            </div>
          </div>
          <p class="job-title-inner">Quality Engineering Co-Op</p>
          <ul>
            <li>Observed an FDA audit of Ethicon Inc, gaining exposure to compliance processes</li>
            <li>
              Supported product validation efforts, ensuring quality standards and specifications
              were met.
            </li>
            <li>
              Assisted in preparing and organizing non-conformance reports, supporting the
              identification and resolution of quality issues.
            </li>
          </ul>
        </div>
      </section>

      <section class="education-section">
        <h3 class="section-title">EDUCATION</h3>
        <div class="education-item">
          <div class="education-header">
            <p><strong>Indiana University Southeast</strong>, New Albany, IN</p>
            <p>2014-2020</p>
          </div>
          <p>BA – General Studies, Minor Informatics</p>
        </div>
      </section>

      <section class="portfolio-section">
        <h3 class="section-title">PORTFOLIO</h3>
        <ul>
          <li>
            <a target="_blank" href="https://www.paramountminus.me/#/" class="link"
              >Paramount+ Clone</a
            >
          </li>
          <li>
            <a target="_blank" href="https://www.conradeyecenters.com/" class="link"
              >Doctors Office Website</a
            >
          </li>
          <li>
            <a target="_blank" href="https://www.fsw.edu/academics/schedule_search" class="link"
              >Class Schedule Search</a
            >
          </li>
        </ul>
      </section>

      <section class="skills-section">
        <h3 class="section-title">TECHNICAL SKILLS</h3>
        <p>
          <strong>Languages & Frameworks:</strong> Python, Django, PHP, Laravel, JavaScript, React,
          Next.js, Vue, CSS, Tailwind, Bootstrap, GraphQL, Elixir
        </p>
        <p><strong>Databases:</strong> PostgreSQL, MongoDB</p>
        <p><strong>Cloud Services:</strong> AWS Suite, Third-Party REST APIs</p>
        <p>
          <strong>Tools:</strong> Microsoft Visual Studio, Git, HashiCorp Vault, Linux, GitHub,
          Bitbucket, Jira, Agile methodologies, Servicenow
        </p>
        <p>
          <strong>Additional Skills:</strong> Proficient in software architectures, code reviews,
          computer science fundamentals, and database management
        </p>
      </section>
    </div>
  </div>
</template>

<script>
import parchment from '@/assets/parchment.jpg'
export default {
  name: 'ResumeComponent',
  data() {
    return {
      parchment,
    }
  },
}
</script>

<style scoped>
.container {
  display: flex;
  justify-content: center;
  font-family: Arial, sans-serif;
  padding: 20px;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  min-height: 100vh;
  width: 100%;
  margin: 0;
}
.resume-wrapper {
  max-width: 800px;
  width: 100%;
  padding: 30px;
}

.resume-header {
  text-align: center;
  margin-bottom: 20px;
}

.resume-header h1 {
  font-size: 28px;
  font-weight: bold;
  margin-bottom: 5px;
}

.contact-info {
  margin: 10px 0;
}

.separator {
  margin: 0 5px;
}

.job-title {
  font-size: 20px;
  font-weight: bold;
  margin-top: 15px;
  padding-bottom: 5px;
}

.experience-section,
.portfolio-section,
.skills-section,
.education-section {
  margin-bottom: 25px;
}

.job {
  margin-bottom: 20px;
}

.job-header {
  display: flex;
  justify-content: space-between;
  align-items: baseline;
  margin-bottom: 5px;
}

.job-location {
  display: flex;
  justify-content: space-between;
  width: 60%;
}

.job-title-inner {
  font-style: italic;
  margin-bottom: 5px;
}

ul {
  list-style-type: disc;
  padding-left: 20px;
  margin-bottom: 15px;
}

.section-title {
  font-weight: bold;
  font-size: 18px;
  padding-bottom: 5px;
  margin-bottom: 10px;
}

.education-header {
  display: flex;
  justify-content: space-between;
  margin-bottom: 5px;
}

.link {
  color: #3f3723;
  text-decoration: none;
}

.link:hover {
  text-decoration: underline;
  background-color: transparent;
}

strong {
  font-weight: bold;
}
</style>
