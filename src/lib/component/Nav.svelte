<script lang="ts">
    // Importation du type de Svelte
    import type { Snippet } from "svelte";

    // Définition du type pour les props de Nav
    type NavType = {
        children: Snippet; // type de variable snippet
    };

    // Déstructuration des props avec le type défini
    let { children }: NavType = $props();
</script>

<!-- Navigation avec des classes utilitaires Tailwind CSS -->
<nav class="flex items-center justify-center border-b-indigo-600 px-8 text-primary-foreground ">
    <!-- Rendu des enfants du composant -->
    {@render children() }
</nav>
