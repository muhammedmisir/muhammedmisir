<h1 align="center">
  Hi, Nice to Meet You! <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="30px">
</h1>

<p align="center">   
  <a href="mailto:muhammed.misir@googlemail.com" target="_blank"><img src="https://img.shields.io/badge/-Email-0D1117?style=for-the-badge&logo=gmail&logoColor=0078D4"></a>
  <a href="https://linkedin.com/in/muhammedmisir" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-0D1117?style=for-the-badge&logo=linkedin&logoColor=0078D4"></a>
</p>

## 🏋 About Me

```typescript
import { Component,  signal, effect } from '@angular/core';

@Component({
  selector: 'app-about-me',
  template: `
    <section class="about-me">
      <h1>Hi there 👋, I'm {{name()}}</h1>
      <p>I am a freelance software engineer based in {{location()}}.</p>
      <p>I regularly write articles on
        <a href="https://frontendbase.com" alt="frontendbase" target="_blank">{{blog()}}</a>
      </p>
      <h3>My Techstack ⚒️</h3>
      <ul>
        <li>Angular</li>
        <li>NextJs</li>
        <li>Java/Spring</li>
        <li>Azure Cloud</li>
      </ul>
    </section>
  `,
  standalone: true
})
export class AboutMeComponent {
  name = signal('Muhammed Misir');
  location = signal('Zurich / Switzerland');
  blog = signal('frontendbase.com');

  constructor() {
    effect(() => {
      console.log(`Greetings from ${this.name()}👋!`);
    });
  }
}
```

