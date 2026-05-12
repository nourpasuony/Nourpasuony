## Hi, I'm Rafnix Guzmán a Python Software Developer 
![]()

```javascript
import { Injectable } from '@nestjs/common';

@Injectable()
export class DeveloperService {
  private readonly username = 'Nour';
  private readonly name = 'Nour mohamed';
  private readonly position = 'Software Developer Nodejs';

  private readonly cv =
    'Nour mohamed CV: https://drive.google.com/file/d/15223Ou80s5kMCbjva5Gfk3R7Pf2JWj1I/view?usp=sharing';

  private readonly code = {
    backend: ['Nodejs', 'Nestjs', 'Expressjs', 'PHP'],
    database: ['PostgreSQL', 'MySQL', 'MongoDB', 'Redis'],
    devops: ['Docker', 'GitHub Actions', 'Linux'],
    frontend: ['HTML','CSS','JavaScript','ReactJS','Redux','Material UI','Tailwind CSS','Bootstrap'],
    tools: ['Git', 'GitHub', 'VS Code', 'Nginx'],
    misc: ['SOLID', 'gRPC'],
  };

  private readonly architecture = ['MVC','Layered','Microservices'];

  toString(): string {
    return `${this.name} | ${this.position}`;
  }

  getPortfolio() {
    return {
      identity: {
        username: this.username,
        name: this.name,
        position: this.position,
      },
      cv: this.cv,
      skills: this.code,
      architecture: this.architecture,
    };
  }
}

const me = new DeveloperService();

console.log(JSON.stringify(me.getPortfolio(), null, 2));

```
