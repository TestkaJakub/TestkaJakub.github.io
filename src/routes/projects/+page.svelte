<script lang="ts">
  import Project from "../../components/project.svelte";

  import TaskfinImage from "$lib/assets/images/taskfin/Taskfin top3 tasks.png";
  import TaskhellImage from "$lib/assets/images/taskhell/Taskhell welcome page.png";
  import KenshiImage from "$lib/assets/images/Kenshi/Kenshi.png";
</script>

<Project
  title="Taskfin"
  date="August 2025"
  links={[['https://github.com/TestkaJakub/taskfin', 'GitHub repository']]}
  technologies={['Next.js', 'TypeScript', 'Prisma']}>
  <p>
  Taskfin is a to do list manager, designed that calculate the priority of a task. Based on the task priority it displays only the most urgent tasks (unless in a specific view where all the tasks are displayed). Made few months prior Taskhell was a to do list manager as well, the difference lies in Taskfin not being a joke project. Taskfin answers my existing problems with to do lists is a simple yet effective way. Current version of Taskfin is a functional MVP, I will leave it like this for some time as I want to focus on other projects.
  </p>
  <img src={TaskfinImage} class="rounded-lg" alt="Taskfin showcase">
</Project>
<Project
  title="Taskhell Backend"
  date="March 2025"
  links={[
    ['https://github.com/Ksawert560/technologieInternetoweFrontend', 'Frontend GitHub repository'],
    ['https://github.com/Ksawert560/technologieInternetoweBackend', 'Backend GitHub repository'],
  ]}
  technologies={['PHP']}>
  <p>
  I was responsible for the backend part of the Taskhell to do list manager. Taskhell is a joke project, the goal of it was to make fun of the hustle culture in which people over rely on tools like to do lists. Taskhell has all the functionalities needed to call it a to do list manager and some that are here either because they are silly or irritating. Backend consist of an REST API that controls things like tasks, lists and users.
  </p>
  <img src={TaskhellImage} class="rounded-lg" alt="Taskhell showcase">
</Project>
<Project title="Spam Email Classification"
  date="February 2025"
  links={[['https://github.com/TestkaJakub/spam-email-classification', 'GitHub repository']]}
  technologies={['Python']}>
  <p>
  It's a second machine learning model I ever did, first one tried to predict if an traffic accident happened, it was for the machine learning classes in CDV and was a failure. I relied on the experience gained when creating the first model to create this one heavily. This project is a binary classification model that categorizes emails as spam or not spam. 
  </p>
</Project>
<Project title="Russian Roulette Simulator"
  date="January 2025"
  links={[['https://github.com/TestkaJakub/russian_roulette', 'GitHub repository']]}
  technologies={['Rust']}>
  <p>
  Though being a simple project for me it renders reaching a certain level of proficiency with Rust programming language I was learning at the time. It's a CLI based russian roulette game simulator.
  </p>
  </Project>
<Project title="WVRN Constant Solver"
  date="January 2025"
  links={[['https://github.com/TestkaJakub/WVRN-constants-solver', 'GitHub repository']]}
  technologies={['Python']}>
  <p>
  A finite state machine and Breadth-first search implementation to find the shortest instruction sequences to generate desired constants on <a href="https://github.com/Q2CK" target="_">@Q2CK's</a> \`WVRN\` Minecraft CPU.
  </p>
</Project>
<Project title="Kenshi"
  date="May - August 2024"
  links={[['https://jakub-testka.itch.io/kenshi', 'Itch.io page']]}
  technologies={['Unity']}>
  <p>
  A collaborative game-dev project made in unity 3D.
  </p>
  <img src={KenshiImage} class="rounded-lg" alt="Kenshi showcase"/>
</Project>
<Project title="Clicker Game"
  date="March 2022"
  links={[
    ['https://github.com/NataliaTI/praktyki2022-marzec-clicker', 'Frontend GitHub repository'],
    ['https://github.com/NataliaTI/praktyki2022-marzec-clicker-api', 'Backend GitHub repository']
  ] as [string, string][]}
  technologies={['PHP', 'JavaScript', 'HTML', 'CSS']}>
  <p>
  A collaborative project, aiming to create a web based clicker game.
  </p>
</Project>
