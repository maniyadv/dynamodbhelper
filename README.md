dynamodbhelper
==============

Helper Class for Dynamo DB in PHP. 
Open DynamoHelper.php for detailed examples written in comments

__EXAMPLES__

> __Put Item__
 

     $putArr 		 = array();
     $dynamoObj 	  = new DynamoHelper();
     $putArr 		 = $dynamoObj->addPutItems("ColumnName1", "ColumnValue1", 'S', $putArr);
     $putArr 		 = $dynamoObj->addPutItems("ColumnName2", "ColumnValue2", 'S', $putArr);
     $putArr 		 = $dynamoObj->addPutItems("ColumnName3", "ColumnValue3", 'S', $putArr);
     $response   	 = $dynamoObj->executeQuery("TableName", $putArr, null, QUERY_PUT_ITEMS);
     var_dump($response);

