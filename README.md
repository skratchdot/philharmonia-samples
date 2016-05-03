# Philharmonia Orchestra Sound Samples

Thousands of free, downloadable sound samples specially recorded by Philharmonia Orchestra players. These samples are suitable for creating any kind of music, no matter what style.

This is just a backup of the original samples from the site:

http://www.philharmonia.co.uk/explore/make_music

## How the backups were generated

1) Visit http://www.philharmonia.co.uk/explore/make_music
2) In Devtools, select the `<optgroup />` containing the instruments.
3) Copy that html element as variable `$p`
4) Run the script:

```javascript
console.clear();
Array.from($p.getElementsByTagName('option')).forEach(function(e){
  var name = e.value.replace('_', '%20');
  console.log(
    'wget  http://www.philharmonia.co.uk/assets/audio/samples/' +
    name + '/' +
    name + '.zip'
  );
});
```

## Download all the samples

```bash
wget http://www.philharmonia.co.uk/assets/audio/samples/banjo/banjo.zip
wget http://www.philharmonia.co.uk/assets/audio/samples/bass%20clarinet/bass%20clarinet.zip
wget http://www.philharmonia.co.uk/assets/audio/samples/bassoon/bassoon.zip
wget http://www.philharmonia.co.uk/assets/audio/samples/cello/cello.zip
wget http://www.philharmonia.co.uk/assets/audio/samples/clarinet/clarinet.zip
wget http://www.philharmonia.co.uk/assets/audio/samples/contrabassoon/contrabassoon.zip
wget http://www.philharmonia.co.uk/assets/audio/samples/cor%20anglais/cor%20anglais.zip
wget http://www.philharmonia.co.uk/assets/audio/samples/double%20bass/double%20bass.zip
wget http://www.philharmonia.co.uk/assets/audio/samples/flute/flute.zip
wget http://www.philharmonia.co.uk/assets/audio/samples/french%20horn/french%20horn.zip
wget http://www.philharmonia.co.uk/assets/audio/samples/guitar/guitar.zip
wget http://www.philharmonia.co.uk/assets/audio/samples/mandolin/mandolin.zip
wget http://www.philharmonia.co.uk/assets/audio/samples/oboe/oboe.zip
wget http://www.philharmonia.co.uk/assets/audio/samples/saxophone/saxophone.zip
wget http://www.philharmonia.co.uk/assets/audio/samples/trombone/trombone.zip
wget http://www.philharmonia.co.uk/assets/audio/samples/trumpet/trumpet.zip
wget http://www.philharmonia.co.uk/assets/audio/samples/tuba/tuba.zip
wget http://www.philharmonia.co.uk/assets/audio/samples/viola/viola.zip
wget http://www.philharmonia.co.uk/assets/audio/samples/violin/violin.zip
wget http://www.philharmonia.co.uk/assets/audio/samples/percussion/percussion.zip
```

## License

The original license is found on the
http://www.philharmonia.co.uk/explore/make_music
site.  It is included below:  
  
  
License: You are free to use these samples as you wish, including releasing them as part of a commercial work. The only restriction is they must not be sold or made available 'as is' (i.e. as samples or as a sampler instrument).

Creative Commons Licence
This work by Philharmonia Orchestra is licensed under a Creative Commons Attribution-ShareAlike 3.0 Unported License.
