# profanewords
 //download the json file
 //read file and store in table
 
        $file = file_get_contents('path to file');
        $profane_words = json_decode($file, true);

        foreach ($profane_words as $words) {
            foreach ($words as $value){
                $value_to_store = $value['word'];
                //sql query here
            }
        }
