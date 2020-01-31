# bigdata2020UTM

## Big data class

### Syllabus contents

* Big Data: It is the storage and processing of large, growing and bulky data sets that a processing software can not manage.
* Open data and private data: Open data are those data that we can find publicly and can be used to analyze patterns, trends. The private ones are those that are confidential since it is information related to a person, a company that must have some privacy.
* Structured and unstructured data: Structured data are those that have a length and format, are those that can be found in a database, the unstructured are those that do not fit the traditional structure of rows and columns (videos, archives of Audio).
* Stored data and moving data: Stored data are those that are structured, are used for the analysis and generation of information. Data in motion are those that are being transmitted on a network, and may suffer alterations.
* Data analysis: It is the process of cleaning, transforming and modeling data to obtain useful information.
* Impact of data analysis: Currently organizations and companies base their decision-making on the analysis of previous data, to perform business and marketing strategies.
* Types of data analysis:
  * 1- Text analysis: It is to do data mining and decipher patterns.
  * 2- Statistical analysis: It is the collection, analysis, interpretation, presentation and modeling of data; There are two descriptive types that analyze complete and numerical and inferential data that can find different conclusions from the same data.
  * 3- Diagnostic analysis: Shows the cause of why things happen from the information found.
  * 4- Predictive analysis: Shows what is likely to happen through the use of previous data.
  * 5- Prescriptive analysis: Combines all types of analysis to determine a decision.

### Other topics

* Docker containers: It is an open source project that automates the deployment of applications within containers.
* MapReduce: It is a framework that provides a parallel and distributed data processing system.
* Hadoop HDFS: Library to make distributed computing for processing large amounts of data. HDFS is the Hadoop file system:
* Apache Spark: It is a programming environment, it works in memory which provides faster processing speed.
* Arquitechture Lambda & Kappa: The main difference is the flow of data processing involved. Lambda has an architecture consisting of the batch layer, the speed layer, the serving layer, unlike kappa is composed of the speed layer and the serving layer

### GitHub Commands
* #### git init: Initialize the repository.
```javascript
Usuario@Jesus MINGW64 ~/Desktop/Hola (master)
$ git init
Reinitialized existing Git repository in C:/Users/Usuario/Desktop/Hola/.git/
}
```
* #### git status: Shows files created, modified from the repository.
```javascript
Usuario@Jesus MINGW64 ~/Desktop/Hola (master)
$ nano bigdata.txt

Usuario@Jesus MINGW64 ~/Desktop/Hola (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        bigdata.txt

nothing added to commit but untracked files present (use "git add" to track)
}
```
* #### git add: Add the file to the staging area.
```javascript
Usuario@Jesus MINGW64 ~/Desktop/Hola (master)
$ git add bigdata.txt
warning: LF will be replaced by CRLF in bigdata.txt.
The file will have its original line endings in your working directory
}
```
* #### git commit - m: Record the changes and add them to the repository.
```javascript
Usuario@Jesus MINGW64 ~/Desktop/Hola (master)
$ git commit
[master b77348c] First project
 1 file changed, 2 insertions(+)
 create mode 100644 bigdata.txt
}
```

* #### git log: Show the commits we have made in our repository.
```javascript
Usuario@Jesus MINGW64 ~/Desktop/Hola (master)
$ git log
commit b77348c433f7a5fae9e5cdd591e22870544f4549 (HEAD -> master)
Author: Jesus Cua <jesuscua05@gmail.com>
Date:   Thu Jan 30 21:39:05 2020 -0600

    First project

}
```

* #### git rm: Remove files from the staging area.
```javascript
Usuario@Jesus MINGW64 ~/Desktop/Hola (master)
$ git rm bigdata.txt
rm 'bigdata.txt'
Usuario@Jesus MINGW64 ~/Desktop/Hola (master)
$ git status
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        deleted:    bigdata.txt

}
```

* #### git mv: It allows us to rename a file.
```javascript
Usuario@Jesus MINGW64 ~/Desktop/Hola (master)
$ git mv Pagina1.html index.html

Usuario@Jesus MINGW64 ~/Desktop/Hola (master)
$ git status
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        deleted:    bigdata.txt
        renamed:    Pagina1.html -> index.html
}
```

* #### git diff: Shows the changes that have been made within the files.
```javascript
Usuario@Jesus MINGW64 ~/Desktop/Hola (master)
$ git diff
diff --git a/index.html b/index.html
index deeaa16..79bc175 100644
--- a/index.html
+++ b/index.html
@@ -4,7 +4,7 @@

     Bienvenidos al curso HTML
 Hola mundo
-
+First project
 </body>

 </html>

}
```

* #### git commit --amend: We can modify the most recent confirmation and even combine changes.
```javascript
Usuario@Jesus MINGW64 ~/Desktop (master)
$ git commit --amend
[master 2bbd870] hoala
 Date: Fri Jan 31 13:03:20 2020 -0600
 1 file changed, 1 insertion(+)
 create mode 100644 index.html
}
```

* #### git reset: Remove commits.
```javascript
Usuario@Jesus MINGW64 ~/Desktop/Hola (master)
$ git reset index.html
Unstaged changes after reset:
M       index.html

Usuario@Jesus MINGW64 ~/Desktop/Hola (master)
$ git status
On branch master
Your branch is ahead of 'origin/master' by 2 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html

no changes added to commit (use "git add" and/or "git commit -a")

}
```
* #### git checkout: Reverse the changes of the files, allow travel to different commits.
```javascript
Usuario@Jesus MINGW64 ~/Desktop/Hola (master)
$ git checkout
M       index.html
Your branch is ahead of 'origin/master' by 2 commits.
  (use "git push" to publish your local commits)

Usuario@Jesus MINGW64 ~/Desktop/Hola (master)
$ git checkout index.html
Updated 1 path from the index

}
```
