### test command
```
http://localhost:10080/notify/graphql?query={songs(album: "ts-fearless"){title,duration}}
```

* create command
```
http://localhost:10080/notify/graphql?query=mutation{createSong(id:"7",album:"ts-fearless",title:"Breathe",duration:"4:23"){title,duration}}
```