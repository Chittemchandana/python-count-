# python-count()
# approach1
s=input()
ch=input()
c=0
for i in range(len(s)):
  if ch==s[i]:
    c=c+1
print(c)

# approach2
s=input()
ch=input()
print(s.count(ch))

# approach3
s=input()
ch=input()
c=0
for i in s:
  if ch==0:
    c=c+1
print(c)

# approach4
s=input()
v="aeiouAEIOU"
for i in range(len(s)):
  if s[i] not in v:
    print("No")
    break
else:
    print("Yes")

# approach5
s=input()
v="aeiouAEIOU"
c=0
for i in range(len(s)):
  if s[i] not in v:
    c=c+1
if c==len(s):
  print("Yes")
else:
  print("No")

# approach6 without range
s=input()
v="aeiouAEIOU"
c=0
for i in v:
  if i in v:
    c=c+1
if c==len(s):
  print("Yes")
else:
  print("No")

# approach7 adding vowels&non-vowels separately
s=input()
v="aeiouAEIOU"
vc=0
cc=0
for i in range(len(s)):
  if s[i].isalpha():
    if s[i] in v:
      vc=vc+1
    else:
      cc=cc+1
print(vc,cc)

# approach8 without range adding vowels&non-vowels separately
s=input()
v="aeiouAEIOU"
vc=0
cc=0
for i in s:
  if i.isalpha():
    if i in v:
      vc=vc+1
    else:
      cc=cc+1
print(vc,cc)


