class Me {
  private name: string;
  private course: string;
  private university: string;
  private job: string;
  private company: string;
  private focus: string;
  private pronouns: string;

  constructor(
    name: string,
    course: string,
    university: string,
    job: string,
    company: string,
    focus: string,
    pronouns: string
  ) {
    this.name = name;
    this.course = course;
    this.university = university;
    this.job = job;
    this.company = company;
    this.focus = focus;
    this.pronouns = pronouns;
  }

  whoIAm(): string {
    return ` 👩‍💻 My name is ${this.name} \n` +
           ` 🎓 I'm a(n) ${this.course} Graduating Student at ${this.university} \n` +
           ` 💼 Currently, I'm working as a(n) ${this.job} at ${this.company} \n` +
           ` 📚 My time is being spent learning ${this.focus} \n` +
           ` 😎 Pronouns: ${this.pronouns}`;
  }
}

const jose = new Me(
  "José Rui",
  "Information Systems",
  "Amazonas Federal University",
  "Back-end Developer",
  "Bemol Digital",
  "Back End Development (Node/Python/.NET/Docker)",
  "He/Him"
);

console.log(jose.whoIAm());
