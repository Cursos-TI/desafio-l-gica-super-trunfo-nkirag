#include <stdio.h>
#include <string.h>

// Desafio Super Trunfo - Países (Nível Intermediário)
// Autor: David Newton (baseado em código original)
// Objetivo: Comparar cartas de cidades com menu interativo e regras de comparação.

int main() {
    // Declaração das variáveis
    char estado1[3], estado2[3], codigo1[3], codigo2[3], cidade1[20], cidade2[20];
    int populacao1, populacao2, pontosT1, pontosT2;
    float area1, area2, pib1, pib2, dens1, dens2, ppc1, ppc2;

    // Entrada de dados para a primeira cidade
    printf("=== Cadastro da Primeira Cidade ===\n");
    printf("Digite a letra do Estado: ");
    scanf("%s", estado1);
    printf("Digite o código da Cidade: ");
    scanf("%s", codigo1);
    printf("Digite o nome da Cidade: ");
    scanf("%s", cidade1);
    printf("Digite o número de habitantes: ");
    scanf("%d", &populacao1);
    printf("Digite a área em km²: ");
    scanf("%f", &area1);
    printf("Digite o PIB (em bilhões): ");
    scanf("%f", &pib1);
    printf("Digite a quantidade de pontos turísticos: ");
    scanf("%d", &pontosT1);

    // Entrada de dados para a segunda cidade
    printf("\n=== Cadastro da Segunda Cidade ===\n");
    printf("Digite a letra do Estado: ");
    scanf("%s", estado2);
    printf("Digite o código da Cidade: ");
    scanf("%s", codigo2);
    printf("Digite o nome da Cidade: ");
    scanf("%s", cidade2);
    printf("Digite o número de habitantes: ");
    scanf("%d", &populacao2);
    printf("Digite a área em km²: ");
    scanf("%f", &area2);
    printf("Digite o PIB (em bilhões): ");
    scanf("%f", &pib2);
    printf("Digite a quantidade de pontos turísticos: ");
    scanf("%d", &pontosT2);

    // Cálculos adicionais
    dens1 = populacao1 / area1;
    dens2 = populacao2 / area2;
    ppc1 = pib1 / populacao1;
    ppc2 = pib2 / populacao2;

    // Exibe os dados das cartas cadastradas
    printf("\n=== Cartas Cadastradas ===\n");
    printf("Carta 1: %s (%s%s)\n", cidade1, estado1, codigo1);
    printf("População: %d | Área: %.2f km² | PIB: %.2f | Pontos turísticos: %d | Densidade: %.2f | PIB per capita: %.2f\n",
           populacao1, area1, pib1, pontosT1, dens1, ppc1);

    printf("\nCarta 2: %s (%s%s)\n", cidade2, estado2, codigo2);
    printf("População: %d | Área: %.2f km² | PIB: %.2f | Pontos turísticos: %d | Densidade: %.2f | PIB per capita: %.2f\n",
           populacao2, area2, pib2, pontosT2, dens2, ppc2);

    // Menu interativo
    int opcao;
    printf("\n=== Escolha o atributo para comparar ===\n");
    printf("1 - População\n");
    printf("2 - Área\n");
    printf("3 - PIB\n");
    printf("4 - Pontos turísticos\n");
    printf("5 - Densidade demográfica\n");
    printf("6 - PIB per capita\n");
    printf("Digite a opção: ");
    scanf("%d", &opcao);

    printf("\n=== Resultado da Comparação ===\n");

    // Switch para escolher o atributo
    switch (opcao) {
        case 1:
            printf("Comparando População:\n");
            printf("%s: %d habitantes | %s: %d habitantes\n", cidade1, populacao1, cidade2, populacao2);
            if (populacao1 > populacao2)
                printf("Vencedora: %s\n", cidade1);
            else if (populacao2 > populacao1)
                printf("Vencedora: %s\n", cidade2);
            else
                printf("Empate!\n");
            break;

        case 2:
            printf("Comparando Área:\n");
            printf("%s: %.2f km² | %s: %.2f km²\n", cidade1, area1, cidade2, area2);
            if (area1 > area2)
                printf("Vencedora: %s\n", cidade1);
            else if (area2 > area1)
                printf("Vencedora: %s\n", cidade2);
            else
                printf("Empate!\n");
            break;

        case 3:
            printf("Comparando PIB:\n");
            printf("%s: %.2f bilhões | %s: %.2f bilhões\n", cidade1, pib1, cidade2, pib2);
            if (pib1 > pib2)
                printf("Vencedora: %s\n", cidade1);
            else if (pib2 > pib1)
                printf("Vencedora: %s\n", cidade2);
            else
                printf("Empate!\n");
            break;

        case 4:
            printf("Comparando Pontos Turísticos:\n");
            printf("%s: %d | %s: %d\n", cidade1, pontosT1, cidade2, pontosT2);
            if (pontosT1 > pontosT2)
                printf("Vencedora: %s\n", cidade1);
            else if (pontosT2 > pontosT1)
                printf("Vencedora: %s\n", cidade2);
            else
                printf("Empate!\n");
            break;

        case 5:
            printf("Comparando Densidade Demográfica (menor vence):\n");
            printf("%s: %.2f | %s: %.2f\n", cidade1, dens1, cidade2, dens2);
            if (dens1 < dens2)
                printf("Vencedora: %s\n", cidade1);
            else if (dens2 < dens1)
                printf("Vencedora: %s\n", cidade2);
            else
                printf("Empate!\n");
            break;

        case 6:
            printf("Comparando PIB per Capita:\n");
            printf("%s: %.2f | %s: %.2f\n", cidade1, ppc1, cidade2, ppc2);
            if (ppc1 > ppc2)
                printf("Vencedora: %s\n", cidade1);
            else if (ppc2 > ppc1)
                printf("Vencedora: %s\n", cidade2);
            else
                printf("Empate!\n");
            break;

        default:
            printf("Opção inválida!\n");
            break;
    }

    return 0;
}
