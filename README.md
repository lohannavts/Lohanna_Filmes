# Lohanna_Filmes

/* Padrão */
:root {
    --rosa-principal: #F52273;
    --cinza-bg: #F5F5F5;
    --cinza-text: #6C6767;

    font-family: 'Roboto', sans-serif;
}

html, body {
    margin: 0;
    padding: 0;
}

.container {
    max-width: 1200px;
    margin-inline: auto;
    padding-inline: 1rem;
}


/* Header */

.header {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 2rem;
    padding: 20px 0;
}

.header p {
    margin: 0;
    font-size: .8rem;
}



/* Professores */
.professores {
    padding: 4rem 0;
    background-color: var(--cinza-bg);
}

.grade-prof {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    justify-content: center;
    gap: 6rem;
}


.prof-item {
    display: flex;
    flex-direction: column;
    gap: .5rem;
}

.img-prof {
    width: 100%;
    max-width: 400px;
}

.nome-prof {
    margin: 0;
    font-weight: 900;
    font-size: 1rem;
}

.valor-prof {
    margin: 0;
    color: var(--rosa-principal);
    font-weight: 700;
    font-size: .8rem;
}

.descricao-prof {
    margin: .8rem 0;
    color: var(--cinza-text);
    font-size: .8rem;
}

.btn-marcar {
    all: unset;
    color: #fff;
    background-color: var(--rosa-principal);
    padding: 1rem;
    font-weight: 900;
    max-width: 230px;
    text-align: center;
    cursor: pointer;
    transition: .4s;
}

.btn-marcar:hover {
    transform: scale(1.03);
}


/* BreakPoints */

@media( max-width: 1400px ) {
    .grade-prof {
        grid-template-columns: repeat(2, 350px);
    }
}


@media( max-width: 992px ) {
    .grade-prof {
        grid-template-columns: 1fr;
    }

    .prof-item {
        align-items: center;
    }
}
