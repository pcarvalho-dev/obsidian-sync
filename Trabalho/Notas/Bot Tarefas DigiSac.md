
URL para listar as chamadas:
	
> [!note]-
> {{URL}}/tickets?query={"distinct":true,"order":[["updatedAt","DESC"]],"where":{"$or":{"startedAt":{"$gte":"2025-08-21T03:00:00.000Z","$lte":"2025-08-29T02:59:00.000Z"},"endedAt":{"$gte":"2025-08-21T03:00:00.000Z","$lte":"2025-08-29T02:59:00.000Z"}}},"include":[{"model":"account"},{"model":"firstMessage","attributes":["id","type","text","timestamp","isFromMe","sent","data","accountId","serviceId","contactId","fromId","toId","userId","ticketId","isFromBot","isFromSync","visible","ticketUserId","ticketDepartmentId","origin","botId","campaignId"]},{"model":"contact","attributes":["id","accountId","name","alternativeName","internalName","serviceId","data","note","personId","status"],"required":true,"where":{"visible":true},"include":[{"model":"service","attributes":["id","name","type","accountId","botId","archivedAt"],"required":true},{"model":"tags","attributes":["id","label","accountId"]},{"model":"person","attributes":["id","name","document","accountId"]},{"model":"thumbAvatar"}]},{"model":"user","attributes":["id","name","email","isSuperAdmin","active","accountId","isFirstLogin","status","timetableId","archivedAt","phoneNumber","data","language","isActiveInternalChat"]},{"model":"department","attributes":["id","name","accountId","archivedAt","distributionId"]},{"model":"ticketTopics","attributes":["id","name","archivedAt"]}],"page":1,"perPage":15}

URL para exportar o PDF:
	
> [!note]-
> https://redeespecialistas.digisac.me/pdf/tickets/20515cf4-3043-47a6-b265-8c8f6992b70d/pt-BR?pdf=1&lng=pt-BR
