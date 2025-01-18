<h1 align="center">SUFU</h1>

<div align="center">
  <kbd align="center">MY Skills</kbd>
</div>

<div align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nextjs/nextjs-original.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-plain.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/rust/rust-plain.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/amazonwebservices/amazonwebservices-original.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/gitlab/gitlab-plain.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-plain.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/flutter/flutter-original.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/debian/debian-original.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-plain-wordmark.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-plain.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/redis/redis-original.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/redux/redux-original.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/ubuntu/ubuntu-plain.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original-wordmark.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/wordpress/wordpress-plain.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/socketio/socketio-original.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/sequelize/sequelize-original.svg" style="width: 44px; height: 44px;" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/graphql/graphql-plain.svg" style="width: 44px; height: 44px;" />
</div>

<div align="center">
  <h2>Projects</h2>
  <ul id="projects-list"></ul>
</div>

<script>
  async function loadProjects() {
    const username = 'chandanbauri';
    try {
      const response = await fetch(`https://api.github.com/users/${username}/repos`);
      if (!response.ok) throw new Error('Failed to fetch repositories');
      const projects = await response.json();

      const projectsList = document.getElementById('projects-list');
      projects.forEach(project => {
        const projectItem = document.createElement('li');
        projectItem.innerHTML = `<a href="${project.html_url}" target="_blank">${project.name}</a>: ${project.description || 'No description provided.'}`;
        projectsList.appendChild(projectItem);
      });
    } catch (error) {
      console.error('Error loading projects:', error);
    }
  }

  loadProjects();
</script>

<div align="center">
  <h2>Connect with Me</h2>
  <a href="https://www.linkedin.com/in/yourprofile" target="_blank">
    <img src="https://img.shields.io/badge/-LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="https://twitter.com/yourprofile" target="_blank">
    <img src="https://img.shields.io/badge/-Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" />
  </a>
  <a href="mailto:your_email@example.com" target="_blank">
    <img src="https://img.shields.io/badge/-Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
</div>

<div align="center">
  <img src="https://gpvc.arturio.dev/chandanbauri" alt="Profile views" />
</div>
