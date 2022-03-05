# Exericios-Eloquent-Javascript

#Looping a triangle
Write a loop that makes seven calls to console.log to output the following triangle:

#
##
###
####
#####
######
#######

```javascript
let count = 0;
let hashtag = "#";

while(count < 7){
  console.log(hashtag);
  hashtag += "#";
  count += 1;
}
```
