# profanewords
 1). Download the json file
 2). Read the file and store the contents in your database
 3). Here's an example using PHP
 
        $file = file_get_contents(storage_path('path to file'));
        $profaneWords = json_decode($file, true);

        foreach ($profaneWords as $words) {
            foreach ($words as $item){
                $valueToStore = $item['word'];
                // TODO enter query to insert the values in your database table
            }
        }
