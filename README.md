# React-cheat-sheet-and-notes
my personal notes and frequently used code snippets for React 


#example of setting the state of one child prop inside an object which is inside of an array (eg. click checkbox for true/false of a list)

handleChange = id => {
      const updateTodos = this.state.todos;
      this.setState({
        todos: updateTodos.map(todo => {
          if (todo.id === id)
            return {
              ...todo,
              completed: !todo.completed
            }
          return todo;
        })
      })
    }

text area is a self closing element (eg. <textarea />)
