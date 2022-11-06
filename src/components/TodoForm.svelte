<script>
    import {addTodo} from "../stores/todoStores"

    let todo = ''
    const handleSubmit = () => {
        addTodo(todo)
        todo = ''
    }
</script>

<main>
    <form class="my-6" on:submit|preventDefault={handleSubmit}>
        <div class="flex flex-col mb-2 text-sm">
            <label class="font-bold text-gray-800" for="todo">Todo</label>
            <input bind:value={todo} class="bind:appearance-none shadow-sm border-gray-200 p-2 
            focus:outline-none focus:border-gray-500 rounded-lg" type="text" name="todo" placeholder="Enter a todo!">
        </div>
        <button class="w-full shadow-sm rounded bg-blue-500 hover:bg-blue-600 text-white py-2 px-4" type="submit">Add Todo</button>
    </form>
</main>