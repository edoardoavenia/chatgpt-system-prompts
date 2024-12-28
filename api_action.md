**API Actions:**  
**1. Retrieve all posts:**  
Namespace: `jsonplaceholder_typicode_com__jit_plugin.getPosts()`  
Returns: List of posts with `userId`, `id`, `title`, and `body`.

**2. Create a new post:**  
Namespace: `jsonplaceholder_typicode_com__jit_plugin.createPost({ userId, title, body })`  
Arguments: Optional `userId`, `title`, and `body`.  
Returns: The created post's details.

**3. Retrieve a specific post by ID:**  
Namespace: `jsonplaceholder_typicode_com__jit_plugin.getPostById({ id })`  
Argument: Required `id` of the post.  
Returns: Post with `userId`, `id`, `title`, and `body`.

**4. Update an existing post:**  
Namespace: `jsonplaceholder_typicode_com__jit_plugin.updatePost({ id, userId, title, body })`  
Arguments: Required `id`, optional `userId`, `title`, and `body`.  
Returns: Updated post's details.

**5. Partially update a post:**  
Namespace: `jsonplaceholder_typicode_com__jit_plugin.partialUpdatePost({ id, title, body })`  
Arguments: Required `id`, optional `title`, and `body`.  
Returns: Partially updated post's details.

**6. Delete a post:**  
Namespace: `jsonplaceholder_typicode_com__jit_plugin.deletePost({ id })`  
Argument: Required `id` of the post.  
Returns: Confirmation of deletion.

**7. Retrieve all comments:**  
Namespace: `jsonplaceholder_typicode_com__jit_plugin.getComments()`  
Returns: List of comments with `postId`, `id`, `name`, `email`, and `body`.

**8. Retrieve all todos:**  
Namespace: `jsonplaceholder_typicode_com__jit_plugin.getTodos()`  
Returns: List of todos with `userId`, `id`, `title`, and `completed`.
