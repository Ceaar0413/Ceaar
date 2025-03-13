# Função para calcular o total da venda
def calcular_total(preco_unitario, quantidade, iva_percentual=14):
    total_sem_iva = preco_unitario * quantidade
    iva = total_sem_iva * (iva_percentual / 100)
    total_com_iva = total_sem_iva + iva
    return total_com_iva, iva

# Função principal de venda
def realizar_venda():
    print("Bem-vindo ao sistema de vendas!")
    
    # Solicitar informações sobre o produto
    nome_produto = input("Digite o nome do produto: ")
    preco_unitario = float(input(f"Digite o preço unitário de {nome_produto} (em AOA): "))
    quantidade = int(input(f"Digite a quantidade de {nome_produto} que deseja compr
