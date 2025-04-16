
2025-04-16  07:19

Status: #adult

Tags: #computer-science #expressjs 

# Query Params

``` js
// Route to get all users

app.get("/api/users", (req, res) => {

	console.log(req.query)
	
	const {
	
	query: { filter, value }
	
	} = req;
	
	if (filter && value) return res.send(
	
	mockUsers.filter((user) => user[filter].includes(value))
	
	);
	
	  
	
	// when filter or value is undefined
	
	return res.send(mockUsers);


});

```



## References

