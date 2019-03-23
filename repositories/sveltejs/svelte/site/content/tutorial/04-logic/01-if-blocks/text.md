---
title: Блок If
---

У HTML нет способа использовать *логику* в виде условных выражений и циклов. А у Svelte есть.

Чтобы отобразить часть разметки при выполнении некоторого условия, мы заключаем ее в блок `if`:

```html
{#if user.loggedIn}
	<button on:click={toggle}>
		Выйти
	</button>
{/if}

{#if !user.loggedIn}
	<button on:click={toggle}>
		Войти
	</button>
{/if}
```

Попробуйте в деле — допишите компонент и понажимайте по кнопке.