public class Livro extends Item {
    private String autor;

    public Livro() {
        super();
        this.autor = "Desconhecido";
    }

    public Livro(String titulo, int ano, String autor) {
        super(titulo, ano);
        this.autor = autor;
    }

    public String getAutor() {
        return autor;
    }

    public void setAutor(String autor) {
        this.autor = autor;
    }

    public void informacoes() {
        System.out.println("Livro: " + getTitulo() + ", de " + getAno()
                + ", do autor: " + autor);
    }

    public void emprestimo() {
        System.out.println("O livro " + getTitulo() + " foi emprestado.");
    }
}