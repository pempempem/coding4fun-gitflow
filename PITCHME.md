# Git Flow

---
@title[Git Flow]

@ul[spaced text-white]
- Workflow Gitflow is model of branching about delivery (write by Vincent Driessen)
- git-flow => git extensions to provide high-level repository operations
@ulend

---
@title[Git Flow : Init]

@snap[north span-50]
@ul[spaced text-white]
- git flow init => Initialize repository 
- Two branchs => master & develop
- master : official version
- develop : integration branch
@ulend
@snapend

@snap[south span-50]
![](assets/img/gitflowinit.png)
@snapend

---
@title[Git Flow : Features]

@snap[west span-50]
@ul[spaced text-white]
- One branch per functionnality (branch pushed to remote after for collaboration)
- feature branch is base to develop branch
- When feature is finished, branch is merged to develop
- feature doesn't use master branch
@ulend
@snapend

@snap[east span-50]
![](assets/img/gitflowfeature.png)
@snapend

---
@title[Git Flow : Releases]

@snap[west span-50]
@ul[spaced text-white]
- Release branch from develop
- No feature, just bug fixing
- Documentation, delivery etc ..
- Merge to master & develop (optional: create tag)
@ulend
@snapend

@snap[east span-50]
![](assets/img/gitflowrelease.png)
@snapend

---
@title[Git Flow : Hotfix]

@snap[west span-50]
@ul[spaced text-white]
- Branch from master (only for production hotfix)
- Merge to master & develop (or current release)
@ulend
@snapend

@snap[east span-50]
![](assets/img/gitflowhotfix.png)
@snapend

---?color=#F6D365
@title[Workshop gitflow]
@box[bg-orange text-white rounded demo-box-pad](Workshop gitflow)

---
@title[Git flow : init]
@snap[west span-70]
### git flow init
@snapend

@snap[east span-30]
![](assets/img/flow_init.png)
@snapend

---
@title[Git flow : list branch]
@snap[west span-70]
### git branch --list
@snapend

@snap[east span-30]
![](assets/img/branch_list_after_init.png)
@snapend

---
@title[Git flow : add new feature]
@snap[west span-70]
### git flow feature start <feature_name>
@snapend

@snap[east span-30]
![](assets/img/add_new_feature.png)
@snapend

---
@title[Git flow : changes feature]
@snap[west span-70]
### git commit -m 'Commit feature'
### git push origin feature/<feature_name>
@snapend

@snap[east span-30]
![](assets/img/push_feature_origin.png)
@snapend

---
@title[Git flow : finish feature]
@snap[west span-70]
### git flow feature finish <feature_name>
### Don't forget to push develop
@snapend

@snap[east span-30]
![](assets/img/finish_feature.png)
@snapend

---
@title[Git flow : add new release]
@snap[west span-70]
### git flow release start <release_version>
@snapend

@snap[east span-30]
![](assets/img/add_new_release.png)
@snapend

---
@title[Git flow : changes release]
@snap[west span-70]
### git commit + push release
@snapend

@snap[east span-30]
![](assets/img/changes_release.png)
@snapend

---
@title[Git flow : finish release]
@snap[west span-70]
### git flow release finish <release_version>
### Don't forget to push develop and master
@snapend

@snap[east span-30]
![](assets/img/finish_release.png)
@snapend