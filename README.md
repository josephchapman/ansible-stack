# ansible

I have no idea what I'm doing.


Install `vagrant` and `virtualbox`, then:
```
$ git clone https://github.com/josephchapman/ansible.git

$ cd ansible

$ vagrant up
```






## Note about excludes

Running `vagrant up` will create the `.vagrant` directory within this project directory.
It contains information you likely don't want to share, such as a private key.
```
.vagrant/machines/default/virtualbox/private_key
```

### Excluding `.vagrant`

Without the exclude, `git` will want to track `.vagrant`:
```
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)

	.vagrant/

nothing added to commit but untracked files present (use "git add" to track)
```
Alter the `.git/info/exclude` file:
```
$ vi .git/info/exclude 

$ tail -n2 .git/info/exclude
# Exclude vagrant info
.vagrant
```
`git` not longer wants to track `.vagrant`:
```
$ git status
On branch master
nothing to commit, working directory clean
```