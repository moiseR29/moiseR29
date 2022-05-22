# Moises Rebatta

```typescript
interface DeveloperSkills {
  [key: string]: Array<string>;
}

interface Developer {
  getName(): string;
  getTitle(): string;
  getLocation(): string;
  getWeb(): string;
  getSkills(): DeveloperSkills;
}

class GitHubDeveloper implements Developer {
  constructor(
    private _name: string,
    private _title: string,
    private _location: string,
    private _web: string,
    private _skills: DeveloperSkills = {}
  ) {}

  getName(): string {
    return this._name;
  }

  getTitle(): string {
    return this._title;
  }

  getWeb(): string {
    return this._web;
  }

  getLocation(): string {
    return this._location;
  }

  getSkills(): DeveloperSkills {
    return this._skills;
  }
}

class Presentation {
  constructor(private _developer: Developer) {}

  private get developer(): Developer {
    return this._developer;
  }

  message(): void {
    console.log(`
Welcome to my profile, My Name is ${this.developer.getName()}.\nI´m ${this.developer.getTitle()}.\nI´m from ${this.developer.getLocation()}
My Skills are:\n ${Object.entries(this.developer.getSkills())
      .map(([key, value]) => `- ${key}: \n  * ${value.join('\n  * ')}\n`)
      .join('')}
    `);
  }
}

const MoisesSkills: DeveloperSkills = {
  backend: [
    'NodeJs (Express, Fastity)',
    'Typescript',
    'GraphQL',
    'REST',
    'Python',
    'CLI',
    'npm (deploy, push, pull libraries)',
    'Extern Services (API Integrations)',
  ],
  database: ['Postgres', 'MySql | MariaDB', 'MongoDB', 'CosmosDB', 'REDIS'],
  devops: [
    'AWS',
    'Terraform',
    'Kubernetes',
    'Linux',
    'Docker',
    'SSH',
    'Travis',
    'Bash',
    'Python',
    'GO',
    'NGINX',
    'NGROK',
    'CircleCI',
    'GitHubAction',
    'Heroku',
  ],
  frontend: ['React'],
  arquitecture: ['Microservices', 'Serverless', 'Events', 'MVC', 'Monolitcs'],
  arquitectureDriven: ['Clean | Hexagonal', 'DDD', 'TDD'],
  tools: ['GIT', 'Github', 'BitBucket', 'Jira', 'Confluence'],
};

const MoisesRebatta = new GitHubDeveloper(
  'Moises Rebatta',
  'Sr Backend && DevOps',
  'Buenos Aires, Argentina',
  'https://www.linkedin.com/in/moises-rebatta-bb1617167',
  MoisesSkills
);

new Presentation(MoisesRebatta).message();

```
```bash
moise@ubuntu: ~
Welcome to my profile, My Name is Moises Rebatta.
I´m Sr Backend && DevOps.
I´m from Buenos Aires, Argentina
My Skills are:
 - backend: 
  * NodeJs (Express, Fastity)
  * Typescript
  * GraphQL
  * REST
  * Python
  * CLI
  * npm (deploy, push, pull libraries)
  * Extern Services (API Integrations)
- database: 
  * Postgres
  * MySql | MariaDB
  * MongoDB
  * CosmosDB
  * REDIS
- devops: 
  * AWS
  * Terraform
  * Kubernetes
  * Linux
  * Docker
  * SSH
  * Travis
  * Bash
  * Python
  * GO
  * NGINX
  * NGROK
  * CircleCI
  * GitHubAction
  * Heroku
- frontend: 
  * React
- arquitecture: 
  * Microservices
  * Serverless
  * Events
  * MVC
  * Monolitcs
- arquitectureDriven: 
  * Clean | Hexagonal
  * DDD
  * TDD
- tools: 
  * GIT
  * Github
  * BitBucket
  * Jira
  * Confluence

```

</br></br>
<h2>💻 Some stats 💻</h2>

![moise's github stats](https://github-readme-stats.vercel.app/api?username=moiseR29&show_icons=true&title_color=fff&icon_color=79ff97&text_color=9f9f9f&bg_color=151515)

## My Skill in Icons

### Backend

<p align="left">
 <a href="https://expressjs.com" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/express/express-original-wordmark.svg" alt="express" width="40" height="40"/> </a>
<a href="https://git-scm.com/" target="_blank"> <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/> </a>
 <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a>
 <a href="https://jestjs.io" target="_blank"> <img src="https://www.vectorlogo.zone/logos/jestjsio/jestjsio-icon.svg" alt="jest" width="40" height="40"/> </a>
 <a href="https://mariadb.org/" target="_blank"> <img src="https://www.vectorlogo.zone/logos/mariadb/mariadb-icon.svg" alt="mariadb" width="40" height="40"/> </a>
 <a href="https://mochajs.org" target="_blank"> <img src="https://www.vectorlogo.zone/logos/mochajs/mochajs-icon.svg" alt="mocha" width="40" height="40"/> </a>
 <a href="https://www.mongodb.com/" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original-wordmark.svg" alt="mongodb" width="40" height="40"/> </a>
 <a href="https://nodejs.org" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original-wordmark.svg" alt="nodejs" width="40" height="40"/> </a>
 <a href="https://www.postgresql.org" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original-wordmark.svg" alt="postgresql" width="40" height="40"/> </a>
 <a href="https://redis.io" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/redis/redis-original-wordmark.svg" alt="redis" width="40" height="40"/> </a>
 <a href="https://www.typescriptlang.org/" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-original.svg" alt="typescript" width="40" height="40"/> </a>
 </p>

### DevOps

<p align="left">
<a href="https://aws.amazon.com" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/amazonwebservices/amazonwebservices-original-wordmark.svg" alt="aws" width="50" height="50"/> </a>
<a href="https://azure.microsoft.com/en-in/" target="_blank"> <img src="https://www.vectorlogo.zone/logos/microsoft_azure/microsoft_azure-icon.svg" alt="azure" width="50" height="50"/> </a>
<a href="https://www.gnu.org/software/bash/" target="_blank"> <img src="https://www.vectorlogo.zone/logos/gnu_bash/gnu_bash-icon.svg" alt="bash" width="50" height="50"/> </a>
<a href="https://circleci.com" target="_blank"> <img src="https://www.vectorlogo.zone/logos/circleci/circleci-icon.svg" alt="circleci" width="50" height="50"/> </a>
<a href="https://www.docker.com/" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original-wordmark.svg" alt="docker" width="50" height="50"/> </a>
<a href="https://golang.org" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/go/go-original.svg" alt="go" width="40" height="40"/> </a>
 <a href="https://kubernetes.io" target="_blank"> <img src="https://www.vectorlogo.zone/logos/kubernetes/kubernetes-icon.svg" alt="kubernetes" width="40" height="40"/> </a>
 <a href="https://www.linux.org/" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="linux" width="40" height="40"/> </a>
 <a href="https://www.nginx.com" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nginx/nginx-original.svg" alt="nginx" width="40" height="40"/> </a>
 <a href="https://www.python.org" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a>
</p>
