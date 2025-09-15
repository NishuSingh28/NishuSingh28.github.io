<!-- Font Awesome for icons -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<style>
  .tab-container {
    display: flex;
    justify-content: flex-end;
    margin-top: 20px;
  }

  .tab-button {
    background-color: #007acc;
    color: white;
    border: none;
    padding: 8px 16px;
    margin-left: 10px;
    border-radius: 5px;
    cursor: pointer;
    font-weight: bold;
  }

  .tab-content {
    display: none;
    margin-top: 30px;
  }

  .tab-content.active {
    display: block;
  }

  .contact-icons a {
    margin: 0 15px;
    color: #007acc;
  }

  .contact-icons i {
    font-size: 2em;
  }
</style>

<div class="tab-container">
  <button class="tab-button" onclick="showTab('about')">About</button>
  <button class="tab-button" onclick="showTab('cv')">CV</button>
</div>

<div id="about" class="tab-content active">
  <h1>Hello World! I’m Nishu Singh</h1>
  <p>
    Master’s in Data Science (ASU) | Master’s in Mathematics<br>
    Worked on NVIDIA’s NeMo project, contributing to large-scale AI and language models.<br>
    Strong in mathematics, data analysis, and problem-solving—turning insights into action.<br>
    A people’s person, curious about international affairs, human psychology, and ideas.<br>
    Love talking, dancing, and when not working, lost in slow, old songs enjoying nature.
  </p>

  <h3>Connect with Me</h3>
  <div class="contact-icons" style="text-align: center;">
    <a href="mailto:nksingh9@asu.edu" title="Email" target="_blank">
      <i class="fa-solid fa-envelope"></i>
    </a>
    <a href="https://github.com/NishuSingh28" title="GitHub" target="_blank">
      <i class="fa-brands fa-github"></i>
    </a>
    <a href="https://www.linkedin.com/in/nishu-kumari-singh-05b36b262/" title="LinkedIn" target="_blank">
      <i class="fa-brands fa-linkedin"></i>
    </a>
  </div>
</div>

<div id="cv" class="tab-content">
  <h2>Download My CV</h2>
  <p style="text-align: center;">
    <a href="Nishu_Singh_CV.pdf" target="_blank" download>
      <button style="padding: 10px 20px; font-size: 16px; background-color: #007acc; color: white; border: none; border-radius: 5px; cursor: pointer;">
        📄 View & Download My CV
      </button>
    </a>
  </p>
</div>

<script>
  function showTab(tabId) {
    document.querySelectorAll('.tab-content').forEach(tab => {
      tab.classList.remove('active');
    });
    document.getElementById(tabId).classList.add('active');
  }
</script>
