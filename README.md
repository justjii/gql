### song
oSELECT * FROM songs
JOIN album ON songs.album = album.id
WHERE songs.album = {album_id}```
```

### test command
```
http://localhost:10080/notify/graphql?query={songs(album: "ts-fearless"){title,duration}}
http://localhost:10080/notify/graphql?query={song(album:%22ts-fearless%22){id,title,duration,album{title}}}
```

* create command
```
http://localhost:10080/notify/graphql?query=mutation{createSong(id:"7",album:"ts-fearless",title:"Breathe",duration:"4:23"){title,duration}}
```

### Author
```
Chih-Han Liu
http://justjii.justdrink.com.tw/
2018.06.03
```
