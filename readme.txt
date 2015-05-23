Read chunk template from a file in assets folder
Read in as string

/////////
//How to read assets file as string
http://stackoverflow.com/questions/16110002/read-assets-file-as-string
StringBuilder buf=new StringBuilder();
    InputStream json=getAssets().open("book/contents.json");
    BufferedReader in=
        new BufferedReader(new InputStreamReader(json, "UTF-8"));
    String str;

    while ((str=in.readLine()) != null) {
      buf.append(str);
    }

    in.close();
	
	
////////////////
//one example
handleChunkFromAssetContent()
just take simple string