#include <stdio.h>

// Definição da estrutura que representa uma carta do Super Trunfo
typedef struct {
    char estado;                  // Letra do estado (A até H)
    char codigo[4];              // Código da carta (ex: A01)
    char nomeCidade[100];        // Nome da cidade
    int populacao;               // Número de habitantes
    float area;                  // Área da cidade em km²
    float pib;                   // Produto Interno Bruto em bilhões
    int pontosTuristicos;        // Número de pontos turísticos
} CartaSuperTrunfo;

int main() {
    // Declaração de duas cartas
    CartaSuperTrunfo carta1;
    CartaSuperTrunfo carta2;

    // ============ Entrada de dados da primeira carta ============
    printf("=== Cadastro da Carta 1 ===\n");

    printf("Informe o Estado (letra de A a H): ");
    scanf(" %c", &carta1.estado);

    printf("Informe o Código da Carta (ex: A01): ");
    scanf("%s", carta1.codigo);

    printf("Informe o Nome da Cidade: ");
    scanf(" %[^\n]", carta1.nomeCidade);

    printf("Informe a População: ");
    scanf("%d", &carta1.populacao);

    printf("Informe a Área (em km²): ");
    scanf("%f", &carta1.area);

    printf("Informe o PIB (em bilhões de reais): ");
    scanf("%f", &carta1.pib);

    printf("Informe o Número de Pontos Turísticos: ");
    scanf("%d", &carta1.pontosTuristicos);

    // ============ Exibição da primeira carta ============
    printf("\nCarta 1:\n");
    printf("Estado: %c\n", carta1.estado);
    printf("Código: %s\n", carta1.codigo);
    printf("Nome da Cidade: %s\n", carta1.nomeCidade);
    printf("População: %d\n", carta1.populacao);
    printf("Área: %.2f km²\n", carta1.area);
    printf("PIB: %.2f bilhões de reais\n", carta1.pib);
    printf("Número de Pontos Turísticos: %d\n", carta1.pontosTuristicos);

    // ============ Entrada de dados da segunda carta ============
    printf("\n=== Cadastro da Carta 2 ===\n");

    printf("Informe o Estado (letra de A a H): ");
    scanf(" %c", &carta2.estado);

    printf("Informe o Código da Carta (ex: B02): ");
    scanf("%s", carta2.codigo);

    printf("Informe o Nome da Cidade: ");
    scanf(" %[^\n]", carta2.nomeCidade);

    printf("Informe a População: ");
    scanf("%d", &carta2.populacao);

    printf("Informe a Área (em km²): ");
    scanf("%f", &carta2.area);

    printf("Informe o PIB (em bilhões de reais): ");
    scanf("%f", &carta2.pib);

    printf("Informe o Número de Pontos Turísticos: ");
    scanf("%d", &carta2.pontosTuristicos);

    // ============ Exibição da segunda carta ============
    printf("\nCarta 2:\n");
    printf("Estado: %c\n", carta2.estado);
    printf("Código: %s\n", carta2.codigo);
    printf("Nome da Cidade: %s\n", carta2.nomeCidade);
    printf("População: %d\n", carta2.populacao);
    printf("Área: %.2f km²\n", carta2.area);
    printf("PIB: %.2f bilhões de reais\n", carta2.pib);
    printf("Número de Pontos Turísticos: %d\n", carta2.pontosTuristicos);

    return 0;
}

