<template>
  <div class="container">
    <div class="resume-wrapper">
      <header class="resume-header">
        <h1>DAVID CONRAD</h1>
        <p>Louisville, KY</p>
        <div class="contact-info">
          <span>david.scott.conrad@gmail.com</span>
          <span class="separator">|</span>
          <span>502-381-3806</span>
          <span class="separator">|</span>
          <a href="#" class="link">LinkedIn</a>
          <span class="separator">|</span>
          <a href="#" class="link">Github</a>
        </div>
        <h2 class="job-title">FRONT END SOFTWARE ENGINEER</h2>
      </header>

      <section class="experience-section">
        <div class="job">
          <div class="job-header">
            <h3>AHEAD</h3>
            <div class="job-location">
              <span>Chicago, IL and NY, NY (Remote)</span>
              <span>Sep 2022-Present</span>
            </div>
          </div>
          <p class="job-title-inner">Software Engineer</p>
          <ul>
            <li>Lead front end modernization of a four year old client portal. Vue.js</li>
            <li>
              Created Google Maps API integration for 1 billion in sales. Pheonix Elixir Framework
            </li>
            <li>Full Stack Dashboard - Big Panda Integration. Vue, Laravel, S3, Mongoldb</li>
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
          <p class="job-title-inner">Software Engineer</p>
          <ul>
            <li>
              Modernized the Class Schedule Search. 15,000 students per semester. React, Codeigniter
              PHP. <a href="#" class="link">Class Schedule Search</a>
            </li>
            <li>Maintained fsw.edu in PHP and React.</li>
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
            <li>Assisted in preparing and organizing non-conformance reports</li>
          </ul>
        </div>
      </section>

      <section class="portfolio-section">
        <h3 class="section-title">PORTFOLIO</h3>
        <ul>
          <li><a href="#" class="link">Paramount+ Clone</a></li>
          <li><a href="#" class="link">Doctors Office Website</a></li>
          <li><a href="#" class="link">Class Schedule Search</a></li>
        </ul>
      </section>

      <section class="skills-section">
        <h3 class="section-title">TECHNICAL SKILLS</h3>
        <p>
          <strong>Languages & Frameworks:</strong> Python, Django, PHP, Laravel, JavaScript, React,
          Next.js, Vue, CSS, Tailwind, Bootstrap, GraphQL, Elixir
        </p>
        <p><strong>Databases:</strong> PostgreSQL, MongoDB</p>
        <p><strong>Cloud Services:</strong> AWS Suite, Third-Party REST APIs, S3</p>
        <p>
          <strong>Tools:</strong> Microsoft Visual Studio, Git, HashiCorp Vault, Linux, GitHub,
          Bitbucket, Jira, Agile methodologies, Servicenow
        </p>
      </section>

      <section class="education-section">
        <h3 class="section-title">EDUCATION</h3>
        <div class="education-item">
          <div class="education-header">
            <p><strong>Indiana University Southeast</strong>, New Albany, IN</p>
            <p>2014-2020</p>
          </div>
          <p>BA – General Studies, Minor Informatics (Business Computer Science)</p>
        </div>
      </section>
    </div>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  justify-content: center;
  font-family: Arial, sans-serif;
  padding: 20px;
  background-image: url(~@/assets/parchment.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  min-height: 100vh;
  width: 100%;
  margin: 0;
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
  border-bottom: 2px solid #ccc;
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
  border-bottom: 2px solid #ccc;
  padding-bottom: 5px;
  margin-bottom: 10px;
}

.education-header {
  display: flex;
  justify-content: space-between;
  margin-bottom: 5px;
}

.link {
  color: #0066cc;
  text-decoration: none;
}

.link:hover {
  text-decoration: underline;
}

strong {
  font-weight: bold;
}
</style>
