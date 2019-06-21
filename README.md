git 分支提交描述：

git init 初始化  
git add README.md  
git commit -m "first commit"  
git remote add origin https://github.com/sunwantong/gitProTest.git //和远程仓库关联起来  
git push -u origin master  //初次提交加 -u参数  


//非初次提交
git add .  
git commit -m 'test'  
git push origin master//push到远程仓库  

//本地建立分支,并将新的分支同步到远程仓库  
git checkout -b  labelCntBranch  (本地建立新的分支并切换到新的分支，labelCntBranch为新的分支名)  
git push origin labelCntBranch  (和远程仓库同步，并在远程仓库建立labelCntBranch分支,如果该远程分支不存在，则会被新建)  

//提交文件到远程labelCntBranch分支  
git add .  
git commit - 'aa'  
git push origin labelCntBranch  

//clone远程仓库，添加新的东西，然后提交(针对主分支)  
git clone https://github.com/sunwantong/gitProTest.git  
进入clone下来的文件夹  
git add 新的东西  
git commit -m 'cc'  
git remote add origin https://github.com/sunwantong/gitProTest.git//本地和远程关联  
git push origin master//提交更新到远程分支  

//clone远程仓库，添加新的东西，然后提交(针对branch分支)  
git clone https://github.com/sunwantong/gitProTest.git  
进入clone下来的文件夹  
git checkout -b labelCntBranch //创建本地分支  
git pull origin labelCntBranch //本地分支与远程分支相关联  
git add 新的东西  
git commit -m 'cc'    
git push origin labelCntBranch//提交更新到远程分支  

git常用命令：  
git log  
git reset --soft versionCode  
git reset --hard versionCode  

git status  
工作区区域(working)  =add>  索引区域(index file)  =commit>  提交区域(commit)


版本回退:  
 git log  
 git reset --soft 6af9459c72aa7c2a82758ec875e9476c096e5df3  
 cola  (利用cola提交,commit)  
 git push origin swt  (不会成功,需要强制push)   
 git push origin swt -f   (强制push)  


