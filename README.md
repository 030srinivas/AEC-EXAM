# AEC-EXAM

-----------------------------------------------------------------------------------------
1.  
	-> git clone <url>
	-> cd <repo>
	-> echo " ">a.txt
	-> git add a.txt
	-> git commit -m "First commit"
	-> git push origin main
------------------------------------------------------------------------------------------

------------------------------------------------------------------------------------------
2.
	-> git clone <url>
	-> cd <repo>
	-> git branch -c "feature-branch"
	-> git checkout feature-branch
	-> echo " ">a.txt
	-> echo " ">b.txt
	-> git add .
	-> git commit -m "done"
	-> git checkout main
	-> git merge feature-branch
	-> git stash
------------------------------------------------------------------------------------------

------------------------------------------------------------------------------------------
3.
	-> git clone <url>
	-> cd <repo>
	-> echo " ">a.txt
	-> git add a.txt
	-> git commit -m "commit in main"
	-> git push origin main
	-> git checkout -b "feature-branch"
	-> echo " ">b.txt
	-> git add b.txt
	-> git commit -m "commit in feature-branch"
	-> git push origin feature-branch
	-> git checkout main
	-> git rebase feature-branch
	-> git push origin main
------------------------------------------------------------------------------------------

------------------------------------------------------------------------------------------
4. 
	-> git clone <url>
	-> cd <repo>
	-> echo " ">a.txt
	-> echo " ">b.txt
	-> git add .
	-> git commit -m "first commit"
	-> git push origin main
	-> git tag v1.0
	-> git push origin v1.0
	-> echo " ">c.txt
	-> git add c.txt
	-> git commit -m "Second commit"
	-> git checkout -b Version1 v1.0
	-> git push origin Version1
	-> git tag // to check tags
------------------------------------------------------------------------------------------

------------------------------------------------------------------------------------------
5.
	-> git clone <url>
	-> cd <repo>
	-> git checkout -b "source-branch"
	-> echo " ">a.txt
	-> git add a.txt
	-> git commit -m "first commit"
	-> echo " ">b.txt 
	-> git add b.txt
	-> git commmit -m "Second commit"
	-> echo " ">c.txt
	-> git add c.txt
	-> git commit -m "Third commit"
	-> git push origin source-branch
	-> git checkout main
	-> git cherry-pick source-branch~2..source-branch
	-> git push origin main
------------------------------------------------------------------------------------------

------------------------------------------------------------------------------------------
6.
	-> git clone <url>
	-> cd <repo>
	-> echo " ">f1.txt
	-> git add f1.txt
	-> git commit -m "First commit"
	-> Commit 4 files
	-> git push origin main
	-> git log
	-> git show <commit_id>
	-> git log --author=" " --since="2024-03-19" --until="2024-03-20"
	-> git log -n 2
------------------------------------------------------------------------------------------





RIGHT TRAINGLE 
def print_right_triangle(rows):
    for i in range(1, rows + 1):
        print("*" * i)

print_right_triangle(5)






INVERTED RIGHT TRIANGLE 
def print_inverted_right_triangle(rows):
    for i in range(rows, 0, -1):
        print("*" * i)

print_inverted_right_triangle(5)




PYRAMID
def print_pyramid(rows):
    for i in range(1, rows + 1):
        print(" " * (rows - i) + "*" * (2 * i - 1))

print_pyramid(5)



INVERTED PYRAMID
def print_inverted_pyramid(rows):
    for i in range(rows, 0, -1):
        print(" " * (rows - i) + "*" * (2 * i - 1))

print_inverted_pyramid(5)
