## 
fig = plt.figure(figsize=(10,4))
fig.set_facecolor('white') ## 캔버스 색상 설정
ax = fig.add_subplot() ## 그림 뼈대(프레임) 생성

ax.plot(실수요.index,실수요['어린이'],marker='o',label='어린이', color='green')

ax.legend() ## 범례

#x축 레이블 회전
plt.xticks(rotation=90)

#그래프 제목 지정
plt.title('계양-연령대별 월별수요(어린이)', fontsize=18)

plt.show()
