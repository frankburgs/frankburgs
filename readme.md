<details><summary>Git cheatsheet</summary><br>

``` bash
$ cls # Clears the screen

$ cd foo # Navigate to folder 'foo'

$ dir # Lists contents of current directory

$ touch "filename" # Creates a file

$ mkdir "foldername" # Creates a folder

$ git clone https/giturl.git # Clone a Github repository locally

$ git init # Creates a repo (.git file)

$ git log  # Shows a history.

$ git status # Tells you the status of the Git

$ git pull # Syncs ❔ local files with cloud files

$ git add filename.ext # "Stages" all files to be committed, use a period to include all fies

$ git commit -m "Meaningful commit message" # "Commits" the file to be pushed

$ git push # "Pushes" the file to the cloud
```

</details>

<details><summary>Tech stack</summary>

``` mermaid
      flowchart LR;
      html([HTML]) --> Style;

      subgraph Style;
        direction LR;
        CSS([CSS]) --> Tailwind([Tailwind<br/>componentless]);
        CSS --> Bootstrap([Bootstrap<br/>w/ components]);
      end;
      
      subgraph Frameworks;
        direction TB
        js([Javascript])
        react([React])
        vite([Vite])
      end;

      Style --> Frameworks;

      subgraph Libraries;
        direction LR
        merm([Mermaid])
        math([MathJax])
      end;

      Frameworks --> Libraries;

      Libraries --> gh([Git<br/>GitHub]);
      gh --> node([Node<br/>PG]);
      node --> sql[(Postgresql)];
      class html,js,vite,react,gh,node,sql,merm,math,Frameworks,Libraries,Style,CSS,Tailwind,Bootstrap cssClass;
      classDef cssClass fill:black,stroke:aqua,color:white;
```

</details>