# Coffe2
def leer_datos():
    N=int(input())
    cafe=[]
    for i in range(N):
        x=list(map(int, input().split()))
        cafe.append(x)
    return cafe

def factor_calidad():
    cafe = leer_datos()
    calidad=[]
    for i in range(len(cafe)):
        if cafe[i][0] >= 10 <= 12 and cafe[i][1]<= 18 and cafe[i][2]>= 15 and cafe[i][3]<= 92:
            calidad.append(cafe[i][4])
    if len(calidad)==0:
        print("NO DISPONIBLE")
    else:
        for i in range (len(calidad)):
            print(calidad[i])

factor_calidad()
