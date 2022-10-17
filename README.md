# StudentInfoManager

## backend setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### the Init of databases

```sql
SET NAMES utf8mb4;
SET FOREIGN_KEY_CHECKS = 0;

-- ----------------------------
-- Table structure for user
-- ----------------------------
DROP TABLE IF EXISTS `user`;
CREATE TABLE `user`  (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `name` varchar(255) CHARACTER SET gbk COLLATE gbk_chinese_ci NOT NULL,
  `age` int(11) NOT NULL,
  `sex` varchar(255) CHARACTER SET gbk COLLATE gbk_chinese_ci NOT NULL,
  PRIMARY KEY (`id`) USING BTREE
) ENGINE = InnoDB AUTO_INCREMENT = 11 CHARACTER SET = gbk COLLATE = gbk_chinese_ci ROW_FORMAT = Compact;

-- ----------------------------
-- Records of user
-- ----------------------------
INSERT INTO `user` VALUES (1, 'tom', 20, '男');
INSERT INTO `user` VALUES (2, 'mary', 20, '女');
INSERT INTO `user` VALUES (3, 'jack', 21, '男');
INSERT INTO `user` VALUES (5, 'test', 20, '未知');
INSERT INTO `user` VALUES (8, 'tom', 20, '男');
INSERT INTO `user` VALUES (9, 'add', 20, '未知');
INSERT INTO `user` VALUES (10, 'Saly', 11, '女');

SET FOREIGN_KEY_CHECKS = 1;

```

